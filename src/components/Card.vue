<template>
  <div>
    <Menu>
      <Logo></Logo>
    </Menu>
  </div>
</template>

<script>
import styled from "vue-styled-components";

export const Menu = styled.div`
  display: flex;
  justify-content: space-between;
  max-width: 900px;
  padding: 25px 0;
  margin: 0 auto;
  background-color: #011;
`;

export const Logo = styled.h1`
  color: #fff;
  padding-left: 10px;
`;

export const Banner = styled.section`
  width: 100vw;
  height: 30vh;
  background-color: cornflowerblue;
`;

export default {
  name: "Card",
  components: {
    Menu,
    Logo,
  },
};
</script>
<style scoped>
</style>
