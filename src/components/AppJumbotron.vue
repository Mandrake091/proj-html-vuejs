<template>
<jumbotron>
<div class="background">

<div class="container-fluid m-auto">
    <div class="row m-auto">
        <div class="col-6">
            <h4>Certified fitness professional</h4>
            <h1>Take control of your healt</h1><br>
            <i class="fa-solid fa-angle-up"></i>
            <i class="fa-solid fa-angle-up"></i>
            <i class="fa-solid fa-angle-up"></i>
            <p>Curabitur non nulla sit amet nisl tempus convallis quis ac lectur dolor sit amet.</p><br>
            <button class="btn-youtube btn rounded-pill p-3">
                <i class="fa-brands fa-youtube"></i>
                Visit my YouTube channel
            </button>
               <button class="btn-buy btn rounded-pill p-3 border-2 border-secondary">
               Buy Avada today
               <i class="fa-solid fa-arrow-right"></i>               
            </button>
        </div>
          <div class="col-6">
            <h1>ciao</h1>
        </div>

    </div>
</div>
</div>
 </jumbotron>
</template>

<script>
export default {
    name:"AppJumbotron",

}
</script>

<style lang="scss" scoped>
@import "../style/generals.scss";

.background{
    position: relative;
    height: calc(100vh - 20vh);
    background-image: url(../assets/images/slider82x-scaled.jpg);
    background-size: cover;
    background-position: top right;
    background-repeat: no-repeat;
    box-shadow: inset 700px 0px 200px black;
}
.container{
    margin: 0 auto;
    position: absolute;
    top: 0;
    left: 0;
}
.btn-youtube{
    background-color: $button-color;
}
.btn{
    margin-right: 30px;
    color: $primary-text;
    &:hover.btn-youtube{
        background-color: $icon-color;
        color: $primary-text;
    }
     &:hover.btn-buy{
        background-color: white;
        color: $bg-navbar;
    } 
}
.row{
    width: 80%;
    margin: 0 auto;
}

</style>