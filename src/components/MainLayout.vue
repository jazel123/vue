<script setup>
import { onMounted } from 'vue';
import Header from '../components/Header.vue';
import Footer from '../components/Footer.vue';



onMounted(() => {
    // Page Title
    document.title = 'Portfolio';
})
</script>

<template>
    <Header />

    <main class="mx-auto max-w-screen-xl px-12 py-6">
        <slot />
    </main>

    <Footer />
</template>
