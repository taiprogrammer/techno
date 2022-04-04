<template>
  <div id="app">
    <Home />
  </div>
</template>

<script>
import Home from "../src/view/Home.vue";
export default {
  name: "App",
  components: {
    Home,
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

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

#app {
  font-family: "Roboto";
  background-color: #d1c0bb;
}
</style>
