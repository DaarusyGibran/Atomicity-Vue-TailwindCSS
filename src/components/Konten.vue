<template>
  <div class="Konten">
      <Background></Background>
      <Blog></Blog>
  </div>
</template>

<script>
import Background from './Background.vue'
import Blog from './Blog.vue'

export default {
  name: 'Konten',
  components: {
    Background,
    Blog
  }
}
</script>

<style>
.textjumbo {
  margin-top: -700px;
  margin-left: 70px;
  position: absolute;
}
.Judul-Blog {
margin-bottom: -30px;
}
</style>
