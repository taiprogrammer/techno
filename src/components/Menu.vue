<template>
  <div>
    <Nav>
      <Container>
        <div>
          <Logo>Make Your Art</Logo>
        </div>
        <div>
          <SearchBar placeholder="search" class="my-input" />
        </div>
        <div>
          <CustomizedButton class="my-btn">Login</CustomizedButton>
          <CustomizedButton class="my-btn">Sign Up</CustomizedButton>
        </div>
      </Container>
    </Nav>
  </div>
</template>

<script>
import styled from "vue-styled-components";

export const CustomizedButton = styled.button`
  background-color: #f2d0bd;
  cursor: pointer;
  padding: 6px 15px;
  border-radius: 4px;
`;

export const SearchBar = styled.input`
  width: 300px;
  padding: 5px;
  border-radius: 5px;
  border: none;
`;

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
  margin: 0;
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
    SearchBar,
    CustomizedButton,
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

.my-input {
  outline: none;
}

.my-input:placeholder {
  margin-left: 15px;
  color: #d98989;
}

.my-input:focus {
  outline: 1.5px solid #d98989;
}

@media (max-width: 730px) {
  .my-input {
    display: none;
  }
}
</style>
