<template>
  <main>
    <div class="background">
      <div class="container">
        <div class="row justify-content-center">
          <div id="img1" class="col-3 d-flex">
            <div class="card-text">
              <h3>Crossfit workout</h3>
              <p>Push your limits</p>
            </div>
          </div>
          <div id="img1" class="col-3 d-flex">
            <div class="card-text">
              <h3>Crossfit workout</h3>
              <p>Push your limits</p>
            </div>
          </div>
          <div id="img1" class="col-3 d-flex">
            <div class="card-text">
              <h3>Crossfit workout</h3>
              <p>Push your limits</p>
            </div>
          </div>
        </div>
        <div class="row">
            <h3>"How you respond to the challenge in the second half will determine what you become after the game, whether you a winner or a loser</h3>
        </div>
      </div>
    </div>
  </main>
</template>
<script>
export default {
  name: "AppMain",
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
  row-gap: 30px;
  column-gap: 30px;
  position: relative;
  top: -50px;
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
  height: 300px;
  width: 275px;
  background-image: url("../assets/images/service6-2x.jpg");
  background-size: cover;
  box-shadow: inset 0px -50px 100px rgba(0, 0, 0, 0.478);
  border-radius: 0 0 25px 0;
  filter: drop-shadow(5px 5px 10px rgba(0, 0, 0, 0.481));
}
img {
  border-radius: 0 0 50px 0;
  box-shadow: inset 10px 10px black;
}
</style>
