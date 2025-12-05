<script setup lang="ts">
  import FooterView from './components/FooterView.vue';
  import HeaderView from './components/HeaderView.vue';
  import HomeHeroView from './components/home/HomeHeroView.vue';
  import RecommendView from './components/home/RecommendView.vue';
</script>

<template>
  <header>
    <HeaderView></HeaderView>
  </header>
  <main>
    <HomeHeroView></HomeHeroView>
    <RecommendView></RecommendView>
  </main>
  <footer>
    <FooterView></FooterView>
  </footer>
</template>

<style scoped>
  header {
    background-color: #D5D5DD;
    backdrop-filter: blur(40px);
  }
</style>
