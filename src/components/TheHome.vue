<template>
<div class="flex flex-col h-full">
    <nav class="w-6xl">
        <TheNavbar/>
    </nav>
    <main class="w-full mt-5 p-5 relative">
        <MainBody/>
    </main>
</div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import TheNavbar from '@/components/TheNavbar.vue';
import MainBody from '@/components/MainBody.vue'
export default defineComponent({
    components:{TheNavbar,MainBody},
    setup() {
        console.log('hello')
    },
})
</script>
