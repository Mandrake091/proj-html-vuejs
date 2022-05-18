<template>
  <main>
    <div class="background">
      <div class="container-fluid pb-5 mb-5">
        <div class="row justify-content-between align-items-center mb-5">
          <div
            id="img1"
            class="col-12 col-md-6 d-flex justify-content-center align-items-center"
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
          <div class="col-12 col-md-6 ps-5">
            <h5>Tune up your workouts</h5>
            <h1>The best health & fitness advice online</h1>
            <div class="d-flex align-items-center">
              <img
                class="channel-logo"
                src="../assets/images/unnamed.jpg"
                alt=""
              />
              <div>
                <p class="mb-2">ThemeFusion</p>
                <strong
                  data-aos="zoom-in"
                  data-aos-offset="200"
                  data-aos-delay="1000"
                  data-aos-duration="1000"
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
            <button class="btn-youtube btn rounded-pill py-2 m-0">
              <i class="fa-brands fa-youtube"></i>
              Visit my YouTube channel
            </button>
          </div>
        </div>
        <div class="row py-5 justify-content-between">
          <div class="col-4 p-0">
            <h4>Featured playlists</h4>
          </div>
          <div class="col-4 text-end">
            <span>
              View all videos
              <i class="fa-solid fa-angle-right"></i>
            </span>
          </div>
        </div>
        <div
          class="row justify-content-between align-items-center text-center mb-5 gx-5"
        >
          <div
            id="img2"
            class="col-12 col-md-4"
            data-aos="fade-right"
            data-aos-offset="200"
            data-aos-delay="50"
            data-aos-duration="1000"
          >
            <img class="" src="../assets/images/video2-2x.jpg" alt="" />
            <div class="play-button rounded-circle">
              <i class="fa-solid fa-play"></i>
            </div>
            <div class="mt-5">
              <h2>Thighs & glute workout</h2>
              <p>Increase your mobility</p>
            </div>
          </div>

          <div
            id="img3"
            class="col-12 col-md-4"
            data-aos="fade-up"
            data-aos-offset="200"
            data-aos-delay="50"
            data-aos-duration="1000"
          >
            <img class="" src="../assets/images/video7-2x.jpg" alt="" />
            <div class="play-button rounded-circle">
              <i class="fa-solid fa-play"></i>
            </div>
            <div class="mt-5">
              <h2>Lift, firm & perk up</h2>
              <p>Fell young again</p>
            </div>
          </div>
          <div
            id="img4"
            class="col-4 col-12 col-md-4"
            data-aos="fade-right"
            data-aos-offset="200"
            data-aos-delay="50"
            data-aos-duration="1000"
          >
            <img class="" src="../assets/images/video9-2x.jpg" alt="" />
            <div class="play-button rounded-circle">
              <i class="fa-solid fa-play"></i>
            </div>
            <div class="mt-5 d-none d-sm-block">
              <h2>Slim & trim trim your waist</h2>
              <p>Shed those extra pounds</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </main>
</template>
<script>
export default {
  name: "AppSectionCards",
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
.play-button:nth-child(2) {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
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
  row-gap: 40px;
  position: relative;
  top: -60px;
}
.row:nth-child(2) {
  width: 80%;
  margin: 0 auto;
}
.row:nth-child(3) {
  position: relative;
  width: 80%;
  margin: 0 auto;
}
.channel-logo {
  margin: 5px;
  width: 50px;
  height: 50px;
}
.phrase {
  color: $primary-text;
}

#img1 {
  position: relative;
  height: 500px;
  background-size: cover;
  background-image: url("../assets/images/service15-2x.jpg");
  // background-size: 100%;
  box-shadow: inset 0px -50px 100px rgba(0, 0, 0, 0.478);
  border-radius: 0 0 25px 0;
  filter: drop-shadow(5px 5px 10px rgba(0, 0, 0, 0.481));
}
#img2 {
  height: 220px;
  filter: drop-shadow(5px 5px 10px rgba(0, 0, 0, 0.481));
}
#img2 > img {
  border-radius: 0 0 25px 0;
  position: relative;
  width: 100%;
  height: 100%;
  object-fit: cover;
  object-position: center center;
}
#img3 {
  height: 220px;
  filter: drop-shadow(5px 5px 10px rgba(0, 0, 0, 0.481));
}
#img3 > img {
  border-radius: 0 0 25px 0;
  position: relative;
  width: 100%;
  height: 100%;
  object-fit: cover;
  object-position: center center;
}
#img4 {
  height: 220px;
  filter: drop-shadow(5px 5px 10px rgba(0, 0, 0, 0.481));
}
#img4 > img {
  border-radius: 0 0 25px 0;
  position: relative;
  width: 100%;
  height: 100%;
  object-fit: cover;
  object-position: center center;
}
</style>
