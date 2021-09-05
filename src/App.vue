<template>
  <div id="app">
    <header-app />
    <home-app />
    <footer-app />
    <back-to-top />
  </div>
</template>

<script>
import HeaderApp from './components/Header.vue'
import FooterApp from './components/Footer.vue'
import BackToTop from './components/BackToTop.vue'
import HomeApp from './views/Home.vue'

export default {
  name: 'App',
  components: {
    HeaderApp,
    HomeApp,
    FooterApp,
    BackToTop
  }
}
</script>

<style lang="scss">
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

html {
  scroll-behavior: smooth;
}

body {
  background-color: #020202;
  font-family: 'Montserrat', sans-serif;
}
</style>
