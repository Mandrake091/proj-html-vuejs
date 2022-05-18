<template>
  <div class="background mt-5 pt-5">
    <div class="container-fluid">
      <div class="row m-auto text-center text-white align-items-center">
        <div class="col-12 col-md-12">
          <h1
            data-aos="zoom-out-up"
            data-aos-offset="200"
            data-aos-delay="200"
            data-aos-duration="1000"
            >
            "I've failed over and over again in my life. And that is why i succeed."
          </h1>
          <br />
          <div class="arrow fs-2">
            <i class="fa-solid fa-angle-up"></i>
            <i class="fa-solid fa-angle-up"></i>
            <i class="fa-solid fa-angle-up"></i>
          </div>

          <p class="fs-4
          ">
            Curabitur non nulla sit amet nisl tempus convallis quis ac lectur
            dolor sit amet.
          </p>
          <br />
          <button class="btn-youtube btn rounded-pill p-3 px-4 m-0 fw-bold">
            Buy Avada today
            <i class="fa-solid fa-angle-right ms-2"></i>
          </button>
        </div>
      </div>
    </div>
  </div>
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
  height: 80vh;
  background-image: url(../assets/images/banner2-2x.jpg);
  background-size: cover;
  background-position: center center;
  background-repeat: no-repeat;
  box-shadow: inset 0px -200px 500px black;
  transition: 0.5s ease-in;
  &:hover {
    box-shadow: inset (0px -100px 300px) black;
  }
}
h1{
  font-size: 3em;
}
p{
  color: $text-grey;

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
}
.arrow {
  color: $title-color;
}

.row {
  height: 100%;
  width: 80%;
  margin: 0 auto;
}
</style>
