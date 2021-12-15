<template>
  <div id="app">
    <!-- componente header -->
    <Header/>
    <!-- componente main -->
    <Main/>
    <!-- componente footer -->
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer
  }
}
</script>

<style lang="scss">
@import './assets/css/global.scss';
</style>
