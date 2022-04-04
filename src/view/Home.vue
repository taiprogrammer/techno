<template>
  <div>
    <Menu />
    <Carousel class="carousel" v-slot="currentSlide">
      <Slide v-for="(slide, index) in carouselSlides" :key="index">
        <div class="slide-info" v-show="currentSlide">
          <img :src="require(`../assets/${slide}.png`)" alt="" />
          {{ currentSlide === index + 1 }}
          <br />
          {{ index + 1 }}
        </div>
      </Slide>
    </Carousel>
  </div>
</template>
<script>
import Menu from "../components/Menu.vue";
import Carousel from "../components/Carousel.vue";
import Slide from "../components/Slide.vue";

export default {
  data() {
    return {
      carouselSlides: ["bg-1", "bg-2", "bg-3"],
    };
  },
  components: {
    Menu,
    Carousel,
    Slide,
  },
};
</script>
<style scoped>
.carousel {
  max-height: 100vw;
  height: 90vh;
  position: relative;
}

.slide-info {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  max-height: 100%;
  height: 100%;
}

.slide-info img {
  min-width: 100%;
  height: 100%;
  object-fit: cover;
}
</style>