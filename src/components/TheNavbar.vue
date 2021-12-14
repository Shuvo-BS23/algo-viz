<template>
    <div class="w-full h-16 bg-gray-600 text-white flex justify-between items-center p-5">
        <div id="brand" class="text-white">ALGO VIZ</div>
        <div id="menu" class="flex justify-items-center p-4 space-x-4">
            <button class="rounded-md hover:opacity-1 hover:cursor-pointer hover:bg-white-300">Bubble Sort</button>    
            <button class="rounded-md hover:opacity-1 hover:cursor-pointer hover:bg-white-300">marge Sort</button>
            <button class="rounded-md hover:opacity-1 hover:cursor-pointer hover:bg-white-300">....</button>
        </div>
    </div>
</template>
<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
    setup() {
       console.log('nav') 
    },
})
</script>
