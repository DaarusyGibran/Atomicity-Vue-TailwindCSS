<template>
  <div id="app">
    <Konten></Konten>
  </div>
</template>

<script>
import Konten from './components/Konten.vue'

export default {
  name: 'App',
  components: {
    Konten
  }
}
</script>

<style>
html {
    scroll-behavior: smooth;
}
#app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: none;
    color: #2c3e50;
    margin-top: 0;
}
</style>
