<template>
  <div id="navbar" class="container-fluid">
    <div class="inner-navbar d-flex align-items-center row p-2 justify-item-center g-2">
      <div class="col-12 col-md-3 text-center">
        <img id="logo" src="../assets/images/logo-2x.png" alt="" />
      </div>
      <div class="col-12 col-md-6">
        <ul class="m-0 p-0 text-center">
          <li v-for="el in datiNavbar" :key="el.name" class="px-2">
            <p class="m-0">
              {{ el.name }}
              <span class="news" v-if="el.new">New</span>
            </p>
          </li>
        </ul>
      </div>
      <div class="col-12 col-md-2 text-center">
        <button class="btn rounded-pill fw-bold ">Schedule a workout</button>
      </div>
      <div class="col-1 d-md-flex d-none justify-content-end text-end">
        <i class="fa-solid fa-cart-shopping pe-2"></i>
        <i class="fa-solid fa-magnifying-glass"></i>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppHeader",
  data() {
    return {};
  },
  computed: {},
  props: ["datiNavbar"],
};
</script>

<style lang="scss" scoped>
@import "../style/generals.scss";

#navbar {
  background-color: $bg-navbar;
}
#logo {
    max-width: 200px;
    width: 100%;
}
.inner-navbar {
  width: 80%;
  height: 100%;
  margin: auto;
}
.btn {
    font-size: 0.8rem;
    color:$primary-text ;
    background: $button-color;
}
.news {
  background: yellow;
  color: black;
}
.fa-solid{
    color: $primary-text;
}
li {
    cursor: pointer;
    color: $icon-navbar;
    display: inline-block;
    list-style-type: none;
    :hover{
        color:$primary-text
    }
}
</style>
