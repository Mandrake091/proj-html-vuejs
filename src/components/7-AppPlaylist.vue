<template>
  <main>
    <div class="background pb-5">
      <div class="container-fluid pb-5 mb-5">
        <div class="row py-5 justify-content-between">
          <div class="col-4">
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
          class="row justify-content-between align-items-center text-center mb-5"
        >
          <div
            class="col-12 col-md-4"
            data-aos="fade-right"
            data-aos-offset="200"
            data-aos-delay="100"
            data-aos-duration="1000"
          >
            <div id="img1" class="hover-background"></div>

            <div class="mt-5">
              <h3>Thighs & glute workout</h3>
              <p>Increase your mobility</p>
            </div>
          </div>

          <div
            class="col-12 col-md-4"
            data-aos="fade-up"
            data-aos-offset="200"
            data-aos-delay="100"
            data-aos-duration="1000"
          >
            <div id="img2" class="hover-background"></div>

            <div class="mt-5">
              <h3>Lift, firm & perk up</h3>
              <p>Fell young again</p>
            </div>
          </div>
          <div
            class="col-12 col-md-4"
            data-aos="fade-right"
            data-aos-offset=""
            data-aos-delay="100"
            data-aos-duration="1000"
          >
            <div id="img3" class="hover-background"></div>
            <div class="mt-5 d-sm-none d-md-block">
              <h3>Slim & trim trim your waist</h3>
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
  name: "AppPlaylist",
};
</script>

<style lang="scss" scoped>
@import "../style/generals.scss";

.row {
  row-gap: 40px;
}
.row:nth-child(2) {
  width: 100%;
  margin: 0 auto;
}
.row:nth-child(3) {
  width: 100%;
  margin: 0 auto;
}
.container-fluid {
  width: 80%;
  margin: 0 auto;
}
.col-12{
  height: 300px;
}
.hover-background {
  width: 100%;
  height: 220px;
  filter: drop-shadow(5px 5px 10px rgba(0, 0, 0, 0.481));
  background-size: cover;
  background-position: center center;
  transition: 1s ease;
  &#img1 {
    background-image: url("../assets/images/blog4-2x.jpg");
  }
  &#img2 {
    background-image: url("../assets/images/blog1-2x.jpg");
  }
  &#img3 {
    background-image: url("../assets/images/blog3-2x.jpg");
  }
  &:hover {
    box-shadow: inset 0px -50px 100px rgba(149, 149, 255, 0.549);
  }
}
</style>
