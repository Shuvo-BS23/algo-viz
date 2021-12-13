<template>
    <nav class="w-6xl">
        <TheNavbar/>
    </nav>
    <h1 class="text-center">hello world</h1>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import TheNavbar from '@/components/TheNavbar.vue'
export default defineComponent({
    components:{TheNavbar},
    setup() {
        console.log('hello')
    },
})
</script>
