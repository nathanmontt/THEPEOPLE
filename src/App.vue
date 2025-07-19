<script setup>
  import AboutComponent from './layout/AboutComponent.vue';
  import ContactComponent from './layout/ContactComponent.vue';
  import DoingComponent from './layout/DoingComponent.vue';
  import HeaderComponent from './layout/HeaderComponent.vue';
  import HeroComponent from './layout/HeroComponent.vue';
</script>

<template>
  <header>
    <HeaderComponent />
  </header>
  
  <main>
    <HeroComponent />
    <div id="about">
      <AboutComponent />
    </div>
    <div id="doing">
      <DoingComponent />
    </div>
    <div id="contact">
      <ContactComponent />
    </div>
  </main>
</template>

<style scoped>
</style>
