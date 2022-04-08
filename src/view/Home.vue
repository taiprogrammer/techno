<template>
  <div>
    <Menu />
    <Carousel class="carousel" />
  </div>
</template>
<script>
import Menu from "../components/Menu.vue";
import Carousel from "../components/Carousel.vue";

export default {
  components: {
    Menu,
    Carousel,
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