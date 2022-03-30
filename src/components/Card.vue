<template>
  <div>
    <CardWrapper>{{ text }}</CardWrapper>
    <Menu />
  </div>
</template>

<script>
import styled from "vue-styled-components";

export const CardWrapper = styled.p`
  color: red;
`;

export const Menu = styled.div`
  height: 10px;
  background-color: #000;
`;

export default {
  props: {
    text: String,
  },
  name: "Card",
  components: {
    CardWrapper,
    Menu,
  },
};
</script>
<style scoped>
</style>
