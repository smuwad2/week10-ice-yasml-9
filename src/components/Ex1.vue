<script>
import { computed } from 'vue';
import SoundIcon from './subcomponents/SoundIcon.vue'

    //import component
    
    export default { 
        data() {
            return {
                soundLevel: 0
            }
        },
        components:{
            SoundIcon
        }
    }
    
</script>

<template>

   Sound level
    <input type="number" min="0" max="3" v-model="soundLevel"> 
    <!-- TODO: Add Code Here to make use of the component -->
    <sound-icon :level="soundLevel"></sound-icon>

</template>

