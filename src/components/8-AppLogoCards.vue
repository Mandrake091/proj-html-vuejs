<template>
  <main>
    <div class="background pb-5 pt-5 mt-5">
      <div class="container-fluid mb-5">
        <div
          class="row justify-content-between align-items-center text-center mb-5"
        >
          <div
            class="col-12 col-md-3"
            data-aos="fade-right"
            data-aos-offset="100"
            data-aos-delay="50"
            data-aos-duration="1000"
          >
            <img src="../assets/images/sponsor-1-2x.png" alt="" />

            <div>
              <div class="arrow fs-2">
                <i class="fa-solid fa-angle-up"></i>
                <i class="fa-solid fa-angle-up"></i>
                <i class="fa-solid fa-angle-up"></i>
              </div>
              <p class="fs-5">
                Tristique aliquam in nullam habitasse nunc, amet vel
                consectetur. Nulla in suspendisse dolor, alique.
              </p>
              <p class="fw-bold">
                Visit Yoga Studio <i class="fa-solid fa-angle-right ms-2"></i>
              </p>
            </div>
          </div>

          <div
            class="col-12 col-md-3"
            data-aos="zoom-out-down"
            data-aos-offset="100"
            data-aos-delay="50"
            data-aos-duration="1500"
          >
            <img src="../assets/images/sponsor-2-2x.png" alt="" />

            <div>
              <div class="arrow fs-2">
                <i class="fa-solid fa-angle-up"></i>
                <i class="fa-solid fa-angle-up"></i>
                <i class="fa-solid fa-angle-up"></i>
              </div>
              <p class="fs-5">
                Tristique aliquam in nullam habitasse nunc, amet vel
                consectetur. Nulla in suspendisse dolor, alique.
              </p>
              <p class="fw-bold">
                Visit Yoga Studio <i class="fa-solid fa-angle-right ms-2"></i>
              </p>
            </div>
          </div>
          <div
            class="col-12 col-md-3"
            data-aos="zoom-out-up"
            data-aos-offset="100"
            data-aos-delay="50"
            data-aos-duration="1500"
          >
            <img src="../assets/images/sponsor-3-2x.png" alt="" />
            <div>
              <div class="arrow fs-2">
                <i class="fa-solid fa-angle-up"></i>
                <i class="fa-solid fa-angle-up"></i>
                <i class="fa-solid fa-angle-up"></i>
              </div>
              <p class="fs-5">
                Tristique aliquam in nullam habitasse nunc, amet vel
                consectetur. Nulla in suspendisse dolor, alique.
              </p>
              <p class="fw-bold">
                Visit Yoga Studio <i class="fa-solid fa-angle-right ms-2"></i>
              </p>
            </div>
          </div>
          <div
            class="col-12 col-md-3"
            data-aos="fade-left"
            data-aos-offset="100"
            data-aos-delay="50"
            data-aos-duration="1000"
          >
            <img src="../assets/images/sponsor-4-2x.png" alt="" />
            <div class="">
              <div class="arrow fs-1">
                <i class="fa-solid fa-angle-up"></i>
                <i class="fa-solid fa-angle-up"></i>
                <i class="fa-solid fa-angle-up"></i>
              </div>
              <p class="fs-5">
                Tristique aliquam in nullam habitasse nunc, amet vel
                consectetur. Nulla in suspendisse dolor, alique.
              </p>
              <p class="fw-bold">
                Visit Yoga Studio <i class="fa-solid fa-angle-right ms-2"></i>
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </main>
</template>
<script>
export default {
  name: "AppLogoCards",
};
</script>

<style lang="scss" scoped>
@import "../style/generals.scss";

.row {
  row-gap: 80px;
}

.row:nth-child(3) {
  width: 100%;
}
.container-fluid {
  width: 80%;
  margin: 0 auto;
}
.arrow {
  color: $button-color;
}
img {
  max-width: 300px;
  position: relative;
  width: 100%;
  height: 70%;
  object-fit: contain;
  object-position: center center;
  height: 220px;
  filter: drop-shadow(5px 5px 2px rgba(0, 0, 0, 0.481));
}
</style>
