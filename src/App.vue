<template>
  <div id="app">
    <Card text="Taiza Marques" />
  </div>
</template>

<script>
import Card from "./components/Card.vue";

export default {
  name: "App",
  components: {
    Card,
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@100;200;300;400;500;600;700;800;900&family=Roboto:wght@100;300;400;500;700;900&display=swap");

body {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

#app {
  font-family: "Roboto";
}
</style>
