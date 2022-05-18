<template>
  <div class="container-fluid p-0">
    <div class="background">
      <div class="row m-auto align-items-center">
        <div
          class="col-12 col-md-9 h-100 my-auto m-auto d-flex flex-column justify-content-center"
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

          <div class="row">
            <input
              type="text"
              class="form-control rounded-pill col-12 col-md-2 m-0 w-50 m-2"
              aria-label="Sizing example input"
              aria-describedby="inputGroup-sizing-default"
              placeholder="Insert your email..*"
            />

            <button
              class="col-10 col-md-7 btn-youtube btn rounded-pill m-2 p-2 w-25"
            >
              Subscribe
            </button>
          </div>
          <p>
            Curabitur non nulla sit amet nisl tempus convallis quis ac lectur
            dolor sit amet.
          </p>
        </div>
        <div
          class="col-3 d-none d-md-flex h-100 d-flex justify-content-center align-items-center"
        ></div>
      </div>
    </div>

    <div class="background-2 py-5">
      <div class="row justify-content-between pt-5 pb-5">
        <div
          class="col-12 col-md-4 d-flex flex-column text-center border border-primary text-white p-5"
          data-aos="zoom-in-up"
          data-aos-duration="500"
          data-aos-offset="0"
          data-aos-delay="250"
          data-aos-id="super-duper"
        >
          <i class="fa-solid fa-stopwatch-20 fs-1"></i>

          <div class="card-text">
            <div class="pt-2">
              <h4>Team training</h4>
              <h5>Find a partner</h5>
            </div>

            <p class="pt-3">
              Vestibulum, curabitur eu sem nibh ultrices sit nulla adipiscing.
              Nisl sit rames amet senectus eget sed duis vehicula. Tristique
            </p>
            <strong
              >Find a partner <i class="fa-solid fa-angle-right ps-2"></i>
            </strong>
          </div>
        </div>
        <div
          class="col-12 col-md-4 d-flex flex-column text-center border border-primary text-white p-5"
          data-aos="zoom-in-up"
          data-aos-duration="500"
          data-aos-offset="0"
          data-aos-delay="500"
          data-aos-id="super-duper"
        >
          <i class="fa-solid fa-weight-hanging fs-1"></i>
          <div class="card-text">
            <div class="pt-2">
              <h4>Team training</h4>
              <h5>Find a partner</h5>
            </div>

            <p class="pt-3">
              Vestibulum, curabitur eu sem nibh ultrices sit nulla adipiscing.
              Nisl sit rames amet senectus eget sed duis vehicula. Tristique
            </p>
            <strong
              >Find a partner <i class="fa-solid fa-angle-right ps-2"></i>
            </strong>
          </div>
        </div>
        <div
          class="col-12 col-md-4 d-flex flex-column text-center border border-primary text-white p-5"
          data-aos="zoom-in-up"
          data-aos-duration="500"
          data-aos-offset="0"
          data-aos-delay="750"
          data-aos-id="super-duper"
        >
          <i class="fa-solid fa-dumbbell fs-1"></i>
          <div class="card-text">
            <div class="pt-2">
              <h4>Team training</h4>
              <h5>Find a partner</h5>
            </div>

            <p class="pt-3">
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
  height: 60vh;
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
  &:hover.btn-buy {
    background-color: white;
    color: $bg-navbar;
  }
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
}
.row:nth-child(2) {
  width: 80%;
  background-color: $bg-navbar;
}
.background-2 .col-md-4 {
}
h5 {
  color: $title-color;
}
</style>
