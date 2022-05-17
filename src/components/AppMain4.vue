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
            id="img2"
            class="col-12 col-md-4"
            data-aos="fade-right"
            data-aos-offset="200"
            data-aos-delay="100"
            data-aos-duration="1000"
          >
            <img class="" src="../assets/images/blog4-2x.jpg" alt="" />

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
            data-aos-delay="100"
            data-aos-duration="1000"
          >
            <img class="" src="../assets/images/blog1-2x.jpg" alt="" />

            <div class="mt-5">
              <h2>Lift, firm & perk up</h2>
              <p>Fell young again</p>
            </div>
          </div>
          <div
            id="img4"
            class="col-12 col-md-4"
            data-aos="fade-rigth"
            data-aos-offset="200"
            data-aos-delay="100"
            data-aos-duration="1000"
          >
            <img class="" src="../assets/images/blog3-2x.jpg" alt="" />
            <div class="mt-5 d-sm-none d-md-block">
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
  name: "AppMain4",
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

#img2 {
  height: 220px;
  filter: drop-shadow(5px 5px 10px rgba(0, 0, 0, 0.481));
}
#img2 > img {
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
  position: relative;
  width: 100%;
  height: 100%;
  object-fit: cover;
  object-position: center center;
}
</style>
