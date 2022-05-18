<template>
  <main>
    <div class="background">
      <div class="container">
        <div class="row justify-content-around justify-content-lg-between">
          <div
            id="img1"
            class="col-12 col-md-3 col-lg-4 d-flex card-image"
            data-aos="fade-up"
            data-aos-offset="200"
            data-aos-delay="50"
            data-aos-duration="1000"
          >
            <div class="card-text">
              <h3>Crossfit workout</h3>
              <p>Push your limits</p>
            </div>
          </div>
          <div
            id="img2"
            class="col-12 col-md-3 col-lg-4 d-flex card-image"
            data-aos="fade-up"
            data-aos-offset="200"
            data-aos-delay="100"
            data-aos-duration="1500"
          >
            <div class="card-text">
              <h3>Crossfit workout</h3>
              <p>Push your limits</p>
            </div>
          </div>
          <div
            id="img3"
            class="col-12 col-md-3 col-lg-4 d-flex card-image"
            data-aos="fade-up"
            data-aos-offset="200"
            data-aos-delay="150"
            data-aos-duration="2000"
          >
            <div class="card-text">
              <h3>Crossfit workout</h3>
              <p>Push your limits</p>
            </div>
          </div>
        </div>
        <div class="phrase row pt-5 mt-5 pb-4 text-center align-items-center">
          <h2 class="">
            "How you respond to the challenge in the second half will determine
            what you become after the game, whether you a winner or a loser.""
          </h2>
          <p class="fs-2">
            <i class="fa-solid fa-angle-up"></i>
            <i class="fa-solid fa-angle-up"></i>
            <i class="fa-solid fa-angle-up"></i>
          </p>
          <div class="text-white pb-5 mb-5">
            <img
              class="rounded-pill"
              src="../assets/images/avatar-1-2x.jpg"
              alt=""
            />
            <span> Brad Johnson <span class="fw-bold">Las Vegas</span></span>
          </div>
        </div>
      </div>
    </div>
  </main>
</template>
<script>
export default {
  name: "B-AppCards+Bg",
};
</script>

<style lang="scss" scoped>
@import "../style/generals.scss";
.background {
  background: rgb(10, 24, 227);
  background: linear-gradient(
    162deg,
    rgba(10, 24, 227, 1) 0%,
    rgba(255, 0, 18, 1) 100%
  );
  width: 100%;
  height: 100%;
}
.container {
  width: 80%;
}
.row {
  column-gap: 30px;
  row-gap: 20px;
  position: relative;
  top: -50px;
}
.fa-solid {
  color: $title-color;
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

.card-image {
  cursor: pointer;
  width: 300px;
  height: 350px;
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center center;
  box-shadow: inset 0px -50px 100px rgba(0, 0, 0, 0.478);
  border-radius: 0 0 25px 0;
  filter: drop-shadow(5px 5px 10px rgba(0, 0, 0, 0.481));
  :hover {
    transform: scale(1.05);
  }

  &#img1 {
    background-image: url("../assets/images/service6-2x.jpg");
    &:hover {
      transform: scale(1.09);
    }
  }
  &#img2 {
    background-image: url("../assets/images/box1-2x.jpg");
    &:hover {
      transform: scale(1.09);
    }
  }
  &#img3 {
    background-image: url("../assets/images/box3-2x.jpg");
    &:hover {
      transform: scale(1.09);
    }
  }
}

</style>
