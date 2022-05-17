<template>
  <main>
    <div class="background pb-5 pt-5 mt-5">
      <div class="container-fluid mb-5">
        <div
          class="row justify-content-between align-items-center text-center mb-5"
        >
          <div
            id="img2"
            class="col-12 col-md-3"
            data-aos="fade-right"
            data-aos-offset="100"
            data-aos-delay="50"
            data-aos-duration="1000"
          >
            <img class="" src="../assets/images/sponsor-1-2x.png" alt="" />

            <div class="">
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
            id="img3"
            class="col-12 col-md-3"
            data-aos="zoom-out-down"
            data-aos-offset="100"
            data-aos-delay="50"
            data-aos-duration="1500"
          >
            <img class="" src="../assets/images/sponsor-2-2x.png" alt="" />

            <div class="">
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
            id="img4"
            class="col-12 col-md-3"
            data-aos="zoom-out-up"
            data-aos-offset="100"
            data-aos-delay="50"
            data-aos-duration="1500"
          >
            <img class="" src="../assets/images/sponsor-3-2x.png" alt="" />
            <div class="">
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
            id="img4"
            class="col-12 col-md-3"
            data-aos="fade-left"
            data-aos-offset="100"
            data-aos-delay="50"
            data-aos-duration="1000"
          >
            <img class="" src="../assets/images/sponsor-4-2x.png" alt="" />
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
  name: "AppMain6",
};
</script>

<style lang="scss" scoped>
@import "../style/generals.scss";

.row {
  row-gap: 80px;

}
.row:nth-child(2) {

 
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
#img2 {
  height: 220px;
  filter: drop-shadow(5px 5px 10px rgba(0, 0, 0, 0.481));
}
#img2 > img {
  position: relative;
  width: 100%;
  height: 70%;
  object-fit: contain;
  object-position: center center;
}
#img3 {
  height: 220px;
  filter: drop-shadow(5px 5px 10px rgba(0, 0, 0, 0.481));
}
#img3 > img {

  width: 100%;
  height: 70%;
  object-fit: contain;
  object-position: center center;
}
#img4 {
  height: 220px;
  filter: drop-shadow(5px 5px 10px rgba(0, 0, 0, 0.481));
}
#img4 > img {

  width: 100%;
  height: 70%;
  object-fit: contain;
  object-position: center center;
}
#img5 {
  height: 220px;
  filter: drop-shadow(5px 5px 10px rgba(0, 0, 0, 0.481));
}
#img5 > img {

  width: 100%;
  height: 70%;
  object-fit: contain;
  object-position: center center;
}
</style>
