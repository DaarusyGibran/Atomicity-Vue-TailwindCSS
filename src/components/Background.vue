<template>
  <div class="Background">
    <div class="carousel">
      <b-carousel id="carousel-1" v-model="slide"
          :interval="4000"
          controls
          indicators
          img-width="1024"
          img-height="350"
      >
          <b-carousel-slide>
              <template v-slot:img>
              <img
                  class="d-block img-fluid w-100 img-banner"
                  src="../assets/quran1.jpg"
                  alt="image slot"
              >
              </template>
          </b-carousel-slide>
      </b-carousel>
        <textjumbo></textjumbo>
    </div>
    <div class="Judul-Blog">
        <p class="font-sans text-5xl text-black text-center">
            BLOG
        </p>
        <hr>
    </div>
</div>
</template>

<script>
import textjumbo from './TextJumbo1.vue'

export default {
  name: 'Background',
  components: {
    textjumbo
  }
}
</script>

<style>
.Judul-Blog {
margin-bottom: -30px;
}
</style>
