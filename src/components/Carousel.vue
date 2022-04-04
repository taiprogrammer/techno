<template>
  <div class="carousel">
    <slot :currentSlide="currentSlide" />
  </div>
</template>
<script>
import { ref } from "vue";
export default {
  name: "Carousel",
  data() {
    return {
      currentSlide: ref(1),
    };
  },
};
</script>
<style scoped>
</style>
