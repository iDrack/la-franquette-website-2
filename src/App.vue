<script setup>
  import NavbarComponent from './components/NavbarComponent.vue';
  import FooterComponent from './components/FooterComponent.vue';
  import { RouterView } from 'vue-router'
</script>

<template>
    <header>
      <NavbarComponent />
    </header>

    <main>
        <RouterView />
    </main>

    <footer>
      <FooterComponent />
    </footer>
</template>

