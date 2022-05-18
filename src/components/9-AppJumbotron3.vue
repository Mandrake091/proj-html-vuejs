<template>
    <div class="background mt-5 pt-5">
      <div class="container-fluid">
        <div class="row m-auto text-center text-white align-items-center">
          <div class="col-12 col-md-12">
            <div class="play-button rounded-circle m-auto">
              <i class="fa-solid fa-play"></i>
            </div>
            <h1>Crossfit workout of the day.</h1>
            <h4>November 15th, 2019</h4>
            <p>View all videos <i class="fa-solid fa-arrow-right-long"></i></p>
            <br />
          </div>
        </div>
      </div>
    </div>
 
</template>

<script>
export default {
  name: "AppJumbotron3",
};
</script>

<style lang="scss" scoped>
@import "../style/generals.scss";

.background {
  position: relative;
  height: 60vh;
  background-image: linear-gradient(
      150deg,
      rgba(10, 24, 227, 0.5) 0%,
      rgba(255, 0, 18, 0.5) 100%
    ),
    url(../assets/images/banner14-2x.jpg);
  filter: contrast(150%), brightness(60%);
  background-size: cover;
  background-position: center center;
  background-repeat: no-repeat;
  transition: 1s ease;
  &:hover{
    filter: brightness(120%);
  }
}
h1{
  font-size: 4em;
}
h4{
  color: $title-color;
}
.container-fluid {
  height: 100%;
  margin: 0 auto;
  position: absolute;
  top: 0;
  left: 0;
}
.play-button {
  line-height: 60px;
  width: 60px;
  height: 60px;
  background-color: $primary-text;
  color: $button-color;
}

.row {
  height: 100%;
  width: 80%;
  margin: 0 auto;
}
</style>
