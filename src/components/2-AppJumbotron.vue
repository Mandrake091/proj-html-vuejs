<template>
  <div class="background mt-0">
    <div class="info text-center fw-bold d-none d-md-block">
      <div
        class="demos bg-white p-2 mb-2"
        data-aos="zoom-in-left"
        data-aos-duration="1000"
        data-aos-offset="0"
        data-aos-delay="500"
        data-aos-id="super-duper"
      >
        <i class="fa-solid fa-cubes"></i>
        <p class="m-0">Demos</p>
      </div>
      <div
        class="on-sale bg-white p-2"
        data-aos="zoom-in-left"
        data-aos-duration="1000"
        data-aos-offset="0"
        data-aos-delay="500"
        data-aos-id="super-duper"
      >
        <span class="">$</span>
        <span class="fw-bold fs-3">39</span>
        <p class="p-on-sale m-0">On Sale</p>
      </div>
    </div>
    <div class="container-fluid m-auto">
      <div class="row m-auto align-items-center">
        <div
          class="col-12 col-md-8 h-100 my-auto m-auto d-flex flex-column justify-content-center"
        >
          <h5
            class="subtitle"
            data-aos="flip-down"
            data-aos-duration="500"
            data-aos-offset="0"
            data-aos-delay="1000"
            data-aos-id="super-duper"
          >
            Certified fitness professional
          </h5>
          <h1
            class="text-white"
            data-aos="flip-up"
            data-aos-duration="1000"
            data-aos-offset="0"
            data-aos-delay="1500"
          >
            Take control of your healt
          </h1>

          <div class="text-start">
            <i
              class="fa-solid fa-angle-up fs-2"
              data-aos="slide-right"
              data-aos-duration="500"
              data-aos-offset="0"
              data-aos-delay="1700"
            ></i>
            <i
              class="fa-solid fa-angle-up fs-2"
              data-aos="slide-right"
              data-aos-duration="500"
              data-aos-offset="0"
              data-aos-delay="1800"
            ></i>
            <i
              class="fa-solid fa-angle-up fs-2"
              data-aos="slide-right"
              data-aos-duration="500"
              data-aos-offset="0"
              data-aos-delay="1900"
              data-aos-id="super-duper"
            ></i>
          </div>

          <p class="fs-4">
            Curabitur non nulla sit amet nisl tempus convallis quis ac lectur
            dolor sit amet.
          </p>

          <div class="text-start d-flex justify-content-between flex-column flex-md-row align-items-center">
            <button
              class="col-7 col-lg-6 btn-youtube btn rounded-pill m-2 p-3 mx-0"
            >
              <i class="fa-brands fa-youtube"></i>
              Visit my YouTube channel
            </button>
            <button
              class="col-5 col-lg-4 btn-buy btn rounded-pill m-2 border-2 border-secondary p-3 mx-0"
            >
              Buy Avada today
              <i class="fa-solid fa-arrow-right"></i>
            </button>
          </div>
        </div>
        <div
          class="col-4 d-none d-md-flex h-100 d-flex justify-content-center align-items-center"
        >
          <div class="play-button rounded-circle text-center">
            <i class="fa-solid fa-play"></i>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppJumbotron",
};
</script>

<style lang="scss" scoped>
@import "../style/generals.scss";

.background {
  position: relative;
  height: 80vh;
  background-color: $bg-navbar;
  background-image: url(../assets/images/slider82x-scaled.jpg);
  background-size: cover;
  background-position: top right;
  background-repeat: no-repeat;
  box-shadow: inset 600px 0px 100px $bg-navbar;
  transition: 1s ease-in-out;
  &:hover {
    box-shadow: inset 550px 0px 150px $bg-navbar;
  }
}
.container-fluid {
  height: 100%;
  margin: 0 auto;
  position: absolute;
  top: 0;
  left: 0;
}
.col-12 {
  row-gap: 10px;
  column-gap: 10px;
  > p {
    color: $text-grey;
  }
  >h1{
    font-size: 4em;
  }
  .fa-angle-up {
    color: $title-color;
  }
}
.subtitle {
  color: $icon-color;
}
.btn-youtube {
  background-color: $button-color;
}
.btn {
  margin-right: 30px;
  color: $primary-text;
  &:hover.btn-youtube {
    background-color: $icon-color;
    color: $primary-text;
  }
  &:hover.btn-buy {
    background-color: white;
    color: $bg-navbar;
  }
}
.play-button {
  line-height: 60px;
  width: 60px;
  height: 60px;
  background-color: $primary-text;
  color: $button-color;
}
.button {
  height: 30px;
}
.info {
  filter: drop-shadow(2px 2px 5px rgba(0, 0, 0, 0.53));
  z-index: 9999;
  width: 60px;
  height: 150px;
  position: fixed;
  top: 80px;
  right: 20px;
}
.on-sale {
  color: $price;
}
.p-on-sale {
  font-weight: bold;
  color: $info-icon;
}
.demos {
  color: $info-icon;
}
.info > div {
  border-radius: 5px;
}
.row {
  height: 100%;
  width: 80%;
  margin: 0 auto;
}
</style>
