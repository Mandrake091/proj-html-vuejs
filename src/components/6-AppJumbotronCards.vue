<template>
  <div class="container-fluid p-0">
    <div class="background">
      <div class="row m-auto align-items-center">
        <div
          class="col-12 col-md-9 h-100 d-flex flex-column justify-content-center"
        >
          <h5 class="subtitle">Join our mailing list today</h5>
          <h1 class="text-white">
            Inside offers & flash sales in your inbox every week.
          </h1>

          <div class="text-start">
            <i class="fa-solid fa-angle-up fs-2"></i>
            <i class="fa-solid fa-angle-up fs-2"></i>
            <i class="fa-solid fa-angle-up fs-2"></i>
          </div>

          <div class="row aling-items-center justify-content-center">
            <input
              type="text"
              class="form-control rounded-pill col-12 col-lg-4 m-0 p-3 m-2 w-50"
              aria-label="Sizing example input"
              aria-describedby="inputGroup-sizing-default"
              placeholder="Insert your email..*"
            />

            <button class="col-6 col-lg-2 btn-youtube btn rounded-pill m-2 p-3">
              Subscribe
            </button>
          </div>
          <p class="fs-4">
            Curabitur non nulla sit amet nisl tempus convallis quis ac lectur
            dolor sit amet.
          </p>
        </div>
        <div
          class="col-3 d-none d-md-flex h-100 d-flex justify-content-center align-items-center"
        >
        </div>
      </div>
    </div>

    <div class="background-2 py-5">
      <div class="row justify-content-center justify-content-lg-between pt-5 pb-5"
      >
        <div
          class="training-card col-12 col-md-4 d-flex flex-column text-center text-white py-5"
          data-aos="flip-left"
          data-aos-duration="500"
          data-aos-offset="0"
          data-aos-delay="250"
          data-aos-id="super-duper"
        >
          <i class="fa-solid fa-stopwatch-20"></i>

          <div class="card-text">
            <div class="pt-2">
              <h2>Team training</h2>
              <h3>Find a partner</h3>
            </div>

            <p class="pt-3 fs-5 pb-5">
              Vestibulum, curabitur eu sem nibh ultrices sit nulla adipiscing.
              Nisl sit rames amet senectus eget sed duis vehicula. Tristique
            </p>
            <strong
              >Find a partner <i class="fa-solid fa-angle-right ps-2"></i>
            </strong>
          </div>
        </div>
        <div
          class="training-card col-12 col-md-4 d-flex flex-column text-center text-white py-5"
          data-aos="flip-left"
          data-aos-duration="500"
          data-aos-offset="0"
          data-aos-delay="500"
          data-aos-id="super-duper"
        >
          <i class="fa-solid fa-weight-hanging"></i>
          <div class="card-text">
            <div class="pt-2">
              <h2>Team training</h2>
              <h3>Find a partner</h3>
            </div>

            <p class="pt-3 fs-5 pb-5">
              Vestibulum, curabitur eu sem nibh ultrices sit nulla adipiscing.
              Nisl sit rames amet senectus eget sed duis vehicula. Tristique
            </p>
            <strong
              >Find a partner <i class="fa-solid fa-angle-right ps-2"></i>
            </strong>
          </div>
        </div>
        <div
          class="training-card col-12 col-md-4 d-flex flex-column text-center text-white py-5"
          data-aos="flip-left"
          data-aos-duration="500"
          data-aos-offset="0"
          data-aos-delay="500"
          data-aos-id="super-duper"
        >
          <i class="fa-solid fa-dumbbell"></i>
          <div class="card-text">
            <div class="pt-2">
              <h2>Team training</h2>
              <h3>Find a partner</h3>
            </div>

            <p class="pt-3 fs-5 pb-5">
              Vestibulum, curabitur eu sem nibh ultrices sit nulla adipiscing.
              Nisl sit rames amet senectus eget sed duis vehicula. Tristique
            </p>
            <strong
              >Find a partner <i class="fa-solid fa-angle-right ps-2"></i>
            </strong>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppJumbotronCards",
};
</script>

<style lang="scss" scoped>
@import "../style/generals.scss";

.background {
  height: 70vh;
  background-image: url(../assets/images/banner1-2x.jpg);
  background-size: cover;
  background-position: top right;
  background-repeat: no-repeat;
  box-shadow: inset 850px 0px 150px $bg-navbar;
  transition: 1s ease-in-out;
  &:hover {
    box-shadow: inset 550px 0px 150px $bg-navbar;
  }
}
.background-2 {
  background: $bg-navbar;
  height: 100%;
}
.container-fluid {
  height: 100%;
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
div > .fa-solid {
  font-size: 4em;
}
.subtitle {
  color: $icon-color;
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
.row:nth-child(1) {
  height: 100%;
  width: 80%;
  margin: 0 auto;
  row-gap: 30px;
  column-gap: 20px;
}
.row:nth-child(0) {
  width: 100%;
}

.col-md-4 {
  cursor: pointer;
  width: 300px;
  height: 400px;
  border: 3px solid $button-color;
  border-radius: 5px;
  transition: 0.5s ease;
}
.training-card:hover {
  transform: scale(1.08);
}
h3 {
  color: $title-color;
}
h1 {
  font-size: 4em;
}
p {
  color: $text-grey;
}
</style>
