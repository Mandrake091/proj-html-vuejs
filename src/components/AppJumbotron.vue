<template>
  <div class="background mt-0">
    <div class="info text-center fw-bold d-none d-md-block">
      <div class="demos bg-white p-2 mb-2">
        <i class="fa-solid fa-cubes"></i>
        <p class="m-0">Demos</p>
      </div>
      <div class="on-sale bg-white p-2">
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
          <h5 class="subtitle">Certified fitness professional</h5>
          <h1 class="text-white">Take control of your healt</h1>

          <div class="text-start">
            <i class="fa-solid fa-angle-up fs-2"></i>
            <i class="fa-solid fa-angle-up fs-2"></i>
            <i class="fa-solid fa-angle-up fs-2"></i>
          </div>

          <p>
            Curabitur non nulla sit amet nisl tempus convallis quis ac lectur
            dolor sit amet.
          </p>

          <div class="text-center">
            <button class="col-10 col-md-7 btn-youtube btn rounded-pill m-2 p-2">
              <i class="fa-brands fa-youtube"></i>
              Visit my YouTube channel
            </button>
            <button
              class="col-10 col-md-4 btn-buy btn rounded-pill m-2 border-2 border-secondary p-2"
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
  height: 60vh;
  background-color: $bg-navbar;
  background-image: url(../assets/images/slider82x-scaled.jpg);
  background-size: cover;
  background-position: top right;
  background-repeat: no-repeat;
  box-shadow: inset 700px 0px 100px $bg-navbar;
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
  width: 60px;
  height: 150px;
  position: absolute;
  top: 50px;
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
