<template>
    <div class="h-full w-2 self-end">
           <div className="bg-blue-500" :style="{height:height+'%' }"></div>
       </div>
</template>

<script lang="ts">
import { defineComponent, PropType } from 'vue'

export default defineComponent({
    props:{
        height:{
            type:Number as PropType<number>,
            default:10
                
        }
        

    },
    setup() {
        console.log('bar')
    },
})
</script>

<style scoped>

</style>
