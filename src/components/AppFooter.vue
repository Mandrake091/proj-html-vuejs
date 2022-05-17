<template>
  <div class="container-fluid p-0">
    <div class="background-2 pt-5">
      <div class="row justify-content-between pt-5 pb-5">
        <div
          class="col-12 col-md-4 d-flex flex-column text-center text-white p-5"
          data-aos="zoom-in-up"
          data-aos-duration="800"
          data-aos-offset="0"
          data-aos-delay="250"
          data-aos-id="super-duper"
        >
          <img src="../assets/images/logo.png" alt="" />

          <div class="card-text">
            <div class="pt-2">
              <p class="pt-3">
                Vestibulum, curabitur eu sem nibh ultrices sit nulla adipiscing.
                Nisl sit rames amet senectus eget sed duis vehicula. Tristique
              </p>
              <p class="pt-5">
                <i class="fa-brands fa-facebook-f"></i>
                <i class="fa-brands fa-twitter"></i>
                <i class="fa-brands fa-youtube"></i>
                <i class="fa-brands fa-instagram"></i>
                <i class="fa-brands fa-linkedin-in"></i>
              </p>
            </div>
          </div>
        </div>
        <div
          class="col-12 col-md-4 d-flex flex-column text-center text-white p-5"
          data-aos="zoom-in-down"
          data-aos-duration="800"
          data-aos-offset="0"
          data-aos-delay="500"
          data-aos-id="super-duper"
        >
          <div class="card-text text-white">
            <h3>RECENT POSTS</h3>
            <ul>
              <li v-for="el in datiFooter" :key="el.name">
                <i class="fa-solid fa-angle-right"></i> {{ el }}
              </li>
            </ul>
          </div>
        </div>
        <div
          class="col-12 col-md-4 d-flex flex-column text-center text-white p-5"
          data-aos="zoom-in-up"
          data-aos-duration="800"
          data-aos-offset="0"
          data-aos-delay="750"
          data-aos-id="super-duper"
        >
          <div class="card-text">
            <div class="pt-2">
              <h3>CONTACT INFORMATIONS</h3>
              <P>4765 Tipple Road Michigan 48392</P>
              <p>Mobile: 1.800.000.0000</p>
              <p>info@gmail.com</p>
            </div>
          </div>
        </div>
      </div>
      <div class="row text-white text-center">
        <p>
          <i class="fa-solid fa-copyright"></i>
          Copyright 2012 - 2020 | Avada theme by Themefusion | All rights reserved | Powered by <strong class="text-white">Paolo Cannistraro</strong>
        </p>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "AppFooter",
  props: ["datiFooter"],
};
</script>

<style lang="scss" scoped>
@import "../style/generals.scss";
.background-2 {
  background-color: black;
  background-size: cover;
  background-position: center center;
  background-repeat: no-repeat;
  box-shadow: inset 0px -100px 200px black;
}
.container-fluid {
  margin: 0 auto;
}
.fa-brands {
  padding: 5px;
  color: $icon-color;
  font-size: 2em;
}
ul {
  list-style: none;
  padding: 0;

  & > li {
    padding: 10px 0;
  }
}
.row {
  height: 100%;
  width: 80%;
  margin: 0 auto;
  &.row:nth-child(2) {
    height: 60px;
    border-top: 1px grey;
    color: $icon-navbar;
  }
}
p{
    color: $text-grey;
}
</style>
