<template>
  <jumbotron>
    <div class="background mt-5 pt-5">
      <div class="container-fluid">
        <div class="row m-auto text-center text-white align-items-center">
          <div class="col-12 col-md-12">
            <h4>Certified fitness professional</h4>
            <h1>Take control of your healt</h1>
            <br />
            <div class="arrow fs-2">
              <i class="fa-solid fa-angle-up"></i>
              <i class="fa-solid fa-angle-up"></i>
              <i class="fa-solid fa-angle-up"></i>
            </div>

            <p>
              Curabitur non nulla sit amet nisl tempus convallis quis ac lectur
              dolor sit amet.
            </p>
            <br />
            <button class="btn-youtube btn rounded-pill px-5 py-2 m-0 fw-bold">
             Buy Avada today
             <i class="fa-solid fa-angle-right ms-2"></i>
            </button>
          </div>
        </div>
      </div>
    </div>
  </jumbotron>
</template>

<script>
export default {
  name: "AppJumbotron2",
};
</script>

<style lang="scss" scoped>
@import "../style/generals.scss";

.background {
  position: relative;
  height: 60vh;
  background-image: url(../assets/images/banner2-2x.jpg);
  background-size: cover;
  background-position: center center;
  background-repeat: no-repeat;
  box-shadow: inset 0px -100px 200px black;
}
.container-fluid {
  height: 100%;
  margin: 0 auto;
  position: absolute;
  top: 0;
  left: 0;
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
.arrow {
  color: $title-color;
}
.play-button {
  line-height: 60px;
  width: 60px;
  height: 60px;
  background-color: $primary-text;
  color: $button-color;
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
