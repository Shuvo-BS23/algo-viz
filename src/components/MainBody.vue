<template>
        <button>start</button>
        <div v-if="barArray" class="mx-auto border-2 ring-black  w-full h-screen flex justify-center space-x-2 items-stretch">
                <TheBar  v-for="(item, index) of barArray"  :key="index"
                :height="item.height"
                
                />
        </div>
   
</template>

<script lang="ts">
import { defineComponent, onBeforeUpdate, ref } from 'vue'
import TheBar from './TheBar.vue';

export default defineComponent({
    setup() {
        console.log("main");
        const barArray = ref<{height:number,active:boolean}[]>([]);
         for (let i=0;i<70;i++){
             barArray.value.push({height:Math.ceil(Math.random()*(100-10)+10),active:false})
         }

       
        
          
        return {
            barArray,
        };
    },
    components: { TheBar }
})
</script>

<style scoped>

</style>
