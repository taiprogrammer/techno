<template>
  <div id="app">
    <Card />
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

body,
h1,
h2,
ul,
li,
p {
  padding: 0px;
  margin: 0px;
}

#app {
  font-family: "Roboto";
}
</style>
