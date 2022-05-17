<template>
  <jumbotron>
    <div class="container-fluid p-0">
      <div class="background">
        <div class="row m-auto align-items-center justify-content-between">
          <div
            class="col-12 col-md-8 align-content-center justify-content-between"
          >
            <h4>Certified fitness professional</h4>
            <h1>Insider offers & flash sales in your inbox every week.</h1>
            <br />
            <i class="fa-solid fa-angle-up"></i>
            <i class="fa-solid fa-angle-up"></i>
            <i class="fa-solid fa-angle-up"></i>

            <br />
            <div class="input-group justify-content-between">
              <input
                type="text"
                class="form-control rounded-pill"
                placeholder="Insert your e-mail...*"
                aria-label="Recipient's username"
                aria-describedby="button-addon2"
              />
              <button
                class="btn-youtube btn rounded-pill border-2 border-secondary px-5 mx-5"
                type="button"
                id="button-addon2"
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
            class="col-4 d-none d-md-flex h-100 d-flex justify-content-center align-items-center"
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
  </jumbotron>
</template>

<script>
export default {
  name: "AppMain3",
};
</script>

<style lang="scss" scoped>
@import "../style/generals.scss";

.background {
  background-image: url(../assets/images/banner1-2x.jpg);
  background-size: cover;
  background-position: top right;
  background-repeat: no-repeat;
  box-shadow: inset 700px 0px 200px black;
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
