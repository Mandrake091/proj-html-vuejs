<template>
  <div id="navbar" class="container-fluid">
    <div
      class="inner-navbar d-flex align-items-center row p-2 justify-item-center justify-content-sm-between g-2"
    >
      <div class="col-4 col-md-3 d-md-block d-none">
        <img
          class="d-md-block d-none"
          id="logo"
          src="../assets/images/logo-2x.png"
          alt=""
        />
      </div>
      <div class="col-12 col-md-6 d-md-block d-none">
        <div class="dropdown">
          <div class="dropdown-buttons d-flex justify-content-between flex-wrap">
            <button
              class="btn btn-dark bg-dark dropdown-toggle"
              @click="menuVisible = !menuVisible"
              :class="{ show: menuVisible }"
              type="button"
              id="dropdownMenuButton1"
              data-bs-toggle="dropdown"
              :aria-expanded="true"
              v-for="el in datiNavbar"
              :key="el.name"
            >
              {{ el.name }}
              <span class="news" v-if="el.new">New</span>
            </button>
          </div>
          <ul
            class="dropdown-menu bg-dark"
            aria-labelledby="dropdownMenuButton1"
            @click="menuVisible = !menuVisible"
            :class="{ show: menuVisible }"
          >
            <li v-for="el in datiNavbar" :key="el.name">
              <a class="dropdown-item text-white" href="#"> {{ el.name }}</a>
              
            </li>
          </ul>
        </div>
      </div>
      <div class="col-12 d-md-block d-none col-md-2 text-center m-0">
        <button class="btn rounded-pill fw-bold ">Schedule a workout</button>
      </div>
      <div class="col-1 d-md-flex d-none justify-content-end text-end">
        <i class="fa-solid fa-cart-shopping pe-2"></i>
        <i class="fa-solid fa-magnifying-glass"></i>
      </div>

      <div class="d-block d-md-none col-12">
        <div class="d-flex justify-content-between align-items-center">
          <img
            class="w-100"
            id="logo"
            src="../assets/images/logo-2x.png"
            alt=""
          />
          <button
            class="navbar-toggler second-button"
            @click="menuVisible = !menuVisible"
            :class="{ collapsed: menuVisible }"
            type="button"
            data-mdb-toggle="collapse"
            data-mdb-target="#navbarToggleExternalContent10"
            aria-controls="navbarToggleExternalContent10"
            aria-expanded="true"
            aria-label="Toggle navigation"
          >
            <div
              class="animated-icon2 m-0"
              :class="{ open: menuVisible }"
              @click="menuVisible = !menuVisible"
            >
              <span></span><span></span><span></span><span></span>
            </div>
          </button>
        </div>

        <div
          :class="{ show: menuVisible }"
          @click="menuVisible"
          class="collapse"
          id="navbarToggleExternalContent10"
        >
          <div class="row pt-3">
            <ul class="m-0 p-0 text-center">
              <li v-for="el in datiNavbar" :key="el.name" class="px-2">
                <p class="m-0 fs-5">
                  {{ el.name }}
                </p>
              </li>
            </ul>
            <input
              type="text"
              class="form-control rounded-pill w-75 m-auto"
              aria-label="Sizing example input"
              aria-describedby="inputGroup-sizing-default"
              placeholder="Search"
            />
            <button class="btn rounded-pill fw-bold w-50 m-auto">
              Schedule a workout
            </button>
            <div class="text-center">
              <i class="fa-solid fa-cart-shopping pe-2"></i>
              <i class="fa-solid fa-magnifying-glass"></i>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "1-AppNav",
  data() {
    return {
      menuVisible: false,
    };
  },
  methods: {},

  computed: {},
  props: ["datiNavbar"],
};
</script>

<style lang="scss" scoped>
@import "../style/generals.scss";
.navbarToggleExternalContent10 {
  & > div {
    background-color: $bg-navbar;
  }
}
#navbar {
  background-color: $bg-navbar;
}
#logo {
  max-width: 200px;
  width: 100%;
}
.dropdown-buttons{
  row-gap: 5px;
  column-gap: 5px;
}
.inner-navbar {
  width: 80%;
  height: 100%;
  margin: auto;
}
.row {
  row-gap: 20px;
}
.btn {
  font-size: 0.8rem;
  color: $primary-text;
  background: $button-color;
}
.news {
  padding: 0 5px;
  font-weight: bold;
  border-radius: 5px;
  background: yellow;
  color: black;
}
.fa-solid {
  color: $primary-text;
}
li {
  cursor: pointer;
  color: $icon-navbar;
  display: inline-block;
  list-style-type: none;
  :hover {
    color: $primary-text;
  }
}

/* Icon 1 */

.animated-icon1,
.animated-icon2,
.animated-icon3 {
  width: 30px;
  height: 20px;
  position: relative;
  margin: 0px;
  -webkit-transform: rotate(0deg);
  -moz-transform: rotate(0deg);
  -o-transform: rotate(0deg);
  transform: rotate(0deg);
  -webkit-transition: 0.5s ease-in-out;
  -moz-transition: 0.5s ease-in-out;
  -o-transition: 0.5s ease-in-out;
  transition: 0.5s ease-in-out;
  cursor: pointer;
}

.animated-icon1 span,
.animated-icon2 span,
.animated-icon3 span {
  display: block;
  position: absolute;
  height: 3px;
  width: 100%;
  border-radius: 9px;
  opacity: 1;
  left: 0;
  -webkit-transform: rotate(0deg);
  -moz-transform: rotate(0deg);
  -o-transform: rotate(0deg);
  transform: rotate(0deg);
  -webkit-transition: 0.25s ease-in-out;
  -moz-transition: 0.25s ease-in-out;
  -o-transition: 0.25s ease-in-out;
  transition: 0.25s ease-in-out;
}

.animated-icon1 span {
  background: #2d7ef7;
}

.animated-icon2 span {
  background: #e3f2fd;
}

.animated-icon3 span {
  background: #f3e5f5;
}

.animated-icon1 span:nth-child(1) {
  top: 0px;
}

.animated-icon1 span:nth-child(2) {
  top: 10px;
}

.animated-icon1 span:nth-child(3) {
  top: 20px;
}

.animated-icon1.open span:nth-child(1) {
  top: 11px;
  -webkit-transform: rotate(135deg);
  -moz-transform: rotate(135deg);
  -o-transform: rotate(135deg);
  transform: rotate(135deg);
}

.animated-icon1.open span:nth-child(2) {
  opacity: 0;
  left: -60px;
}

.animated-icon1.open span:nth-child(3) {
  top: 11px;
  -webkit-transform: rotate(-135deg);
  -moz-transform: rotate(-135deg);
  -o-transform: rotate(-135deg);
  transform: rotate(-135deg);
}

/* Icon 3*/

.animated-icon2 span:nth-child(1) {
  top: 0px;
}

.animated-icon2 span:nth-child(2),
.animated-icon2 span:nth-child(3) {
  top: 10px;
}

.animated-icon2 span:nth-child(4) {
  top: 20px;
}

.animated-icon2.open span:nth-child(1) {
  top: 11px;
  width: 0%;
  left: 50%;
}

.animated-icon2.open span:nth-child(2) {
  -webkit-transform: rotate(45deg);
  -moz-transform: rotate(45deg);
  -o-transform: rotate(45deg);
  transform: rotate(45deg);
}

.animated-icon2.open span:nth-child(3) {
  -webkit-transform: rotate(-45deg);
  -moz-transform: rotate(-45deg);
  -o-transform: rotate(-45deg);
  transform: rotate(-45deg);
}

.animated-icon2.open span:nth-child(4) {
  top: 11px;
  width: 0%;
  left: 50%;
}

/* Icon 4 */

.animated-icon3 span:nth-child(1) {
  top: 0px;
  -webkit-transform-origin: left center;
  -moz-transform-origin: left center;
  -o-transform-origin: left center;
  transform-origin: left center;
}

.animated-icon3 span:nth-child(2) {
  top: 10px;
  -webkit-transform-origin: left center;
  -moz-transform-origin: left center;
  -o-transform-origin: left center;
  transform-origin: left center;
}

.animated-icon3 span:nth-child(3) {
  top: 20px;
  -webkit-transform-origin: left center;
  -moz-transform-origin: left center;
  -o-transform-origin: left center;
  transform-origin: left center;
}

.animated-icon3.open span:nth-child(1) {
  -webkit-transform: rotate(45deg);
  -moz-transform: rotate(45deg);
  -o-transform: rotate(45deg);
  transform: rotate(45deg);
  top: 0px;
  left: 8px;
}

.animated-icon3.open span:nth-child(2) {
  width: 0%;
  opacity: 0;
}

.animated-icon3.open span:nth-child(3) {
  -webkit-transform: rotate(-45deg);
  -moz-transform: rotate(-45deg);
  -o-transform: rotate(-45deg);
  transform: rotate(-45deg);
  top: 21px;
  left: 8px;
}
</style>
