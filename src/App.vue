<template>
  <div id="app">
    <HeaderTailwind />
    <MainSection />    
    <SubSection />
    <FooterTailwind />

  </div>
</template>

<script>

import HeaderTailwind from './components/layout/HeaderTailwind.vue';
import MainSection from './components/layout/MainSection.vue';
import SubSection from './components/layout/SubSection.vue';
import FooterTailwind from './components/layout/FooterTailwind.vue';

export default {
  name: 'App',
  components: {
    
    HeaderTailwind,
    MainSection,
    FooterTailwind,
    SubSection,
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
@import '@/assets/css/input.css';
@import '@/input.css';
</style>
