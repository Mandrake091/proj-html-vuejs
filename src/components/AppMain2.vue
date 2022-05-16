<template>
  <main>
    <div class="background">
      <div class="container-fluid">
        <div class="row justify-content-between align-items-center">
          <div
            id="img1"
            class="col-6 d-flex justify-content-center align-items-center"
            data-aos="fade-right"
            data-aos-offset="200"
            data-aos-delay="50"
            data-aos-duration="1000"
          >
            <div
              class="play-button rounded-circle text-center"
              data-aos="fade-right"
              data-aos-offset="200"
              data-aos-delay="1000"
              data-aos-duration="500"
            >
              <i class="fa-solid fa-play"></i>
            </div>
          </div>
          <div class="col-6 ps-5">
            <h5>Tune up your workouts</h5>
            <h1>The best health & fitness advice online</h1>
            <div class="d-flex align-items-center">
              <img
                class="channel-logo"
                src="../assets/images/unnamed.jpg"
                alt=""
              />
              <div class="m-0">
                <p class="mb-2">ThemeFusion</p>
                <strong
                  class="bg-danger text-white rounded-2 border border-secondary p-1 pe-0"
                >
                  <i class="fa-brands fa-youtube"></i> YouTube
                  <p
                    class="bg-white text-dark d-inline m-1 p-1 pe-0 me-0 fw-normal"
                  >
                    999+
                  </p>
                </strong>
              </div>
            </div>
            <p>
              Arcu eu facilisi ut quisque placerat nunc habitant. Magna semper
              mauris, venenatis leo integer sit pellentesque.
            </p>
            <button class="btn-youtube btn rounded-pill px-5 py-2">
              <i class="fa-brands fa-youtube"></i>
              Visit my YouTube channel
            </button>
          </div>
        </div>
      </div>
    </div>
  </main>
</template>
<script>
export default {
  name: "AppMain2",
};
</script>

<style lang="scss" scoped>
@import "../style/generals.scss";
.background {
  width: 100%;
  height: 100%;
}
.play-button {
  line-height: 60px;
  width: 60px;
  height: 60px;
  background-color: $primary-text;
  color: $button-color;
}
.btn {
  margin-right: 30px;
  color: $primary-text;
  background-color: $icon-color;
  &:hover.btn-youtube {
    background-color: $button-color;
    color: $primary-text;
  }
}
.row {
  position: relative;
  top: -40px;
}
.channel-logo {
  margin: 5px;
  width: 50px;
  height: 50px;
}
.phrase {
  color: $primary-text;
}
.card-text {
  position: absolute;
  bottom: 10px;
  left: 30px;
  & > h3 {
    margin: 0;
    color: $primary-text;
  }
  & > p {
    font-weight: bold;
    color: $title-color;
  }
}
#img1 {
  height: 500px;
  background-image: url("../assets/images/service15-2x.jpg");
  background-size: 100%;
  box-shadow: inset 0px -50px 100px rgba(0, 0, 0, 0.478);
  border-radius: 0 0 25px 0;
  filter: drop-shadow(5px 5px 10px rgba(0, 0, 0, 0.481));
}
</style>
