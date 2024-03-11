<script setup>
import AboutSection from './_partials/AboutSection.vue';
import ContactSection from './_partials/ContactSection.vue';
import HomeSection from './_partials/HomeSection.vue';
import ProductSection from './_partials/ProductSection.vue';

</script>

<template>

    <section id="home" class="w-full pb-24">
        <HomeSection />
    </section>

    <hr class="divider" >

    <section id="product" class="w-full pb-24">
        <ProductSection />
    </section>

    <hr class="divider">

    <section id="about" class="w-full pb-24">
        <AboutSection />
    </section>

    <hr class="divider">

    <section id="contact" class="w-full pb-24">
        <ContactSection />
    </section>

</template>

<style scoped>
</style>