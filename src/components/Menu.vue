<template>
  <div>
    <Nav>
      <Container>
        <div>
          <Logo>Make Your Art</Logo>
        </div>
        <div>
          <a-input-search placeholder="search" style="width: 300px" />
        </div>
        <div>
          <a-button class="my-btn">Login</a-button>
          <a-button class="my-btn">Sign Up</a-button>
        </div>
      </Container>
    </Nav>
  </div>
</template>

<script>
import styled from "vue-styled-components";

export const Container = styled.div`
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-around;
  width: 90%;
  height: 10vh;
`;

export const Logo = styled.h1`
  color: #f2d0bd;
  font-weight: bold;
`;

export const Nav = styled.div`
  width: 100vw;
  background-color: #1a2226;
`;

export default {
  props: {
    text: String,
  },
  name: "Menu",
  components: {
    Nav,
    Container,
    Logo,
  },
};
</script>
<style scoped>
.my-btn {
  background-color: #f2d0bd;
  color: #474f59;
  border: none;
  margin-right: 5px;
}

.my-btn:hover {
  color: #474f59;
  background-color: #ffffff;
}

.my-btn:focus {
  color: #d98989;
}

.my-btn:active {
  color: #d98989;
}
</style>
