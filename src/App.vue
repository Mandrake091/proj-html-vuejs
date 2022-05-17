<template>
  <div id="app">
    <app-nav :datiNavbar="datiNavbar" />
    <app-jumbotron />
    <app-main />
    <app-main-2 />
    <app-main-3 />
    <app-main-4 />
    <app-jumbotron-2 />
    <app-main-6 />
  </div>
</template>

<script>
import dati from "./dati.json";
import AOS from "aos";
import AppNav from "./components/AppNav.vue";
import AppJumbotron from "./components/AppJumbotron.vue";
import AppMain from "./components/AppMain.vue";
import AppMain2 from "./components/AppMain2.vue";
import AppMain3 from "./components/AppMain3.vue";
import AppMain4 from "./components/AppMain4.vue";
import AppJumbotron2 from "./components/AppJumbotron2.vue";
import AppMain6 from "./components/AppMain6.vue";

export default {
  data() {
    return {
      datiNavbar: dati.navbar,
      datiFooter: dati.recentPosts,
    };
  },
  name: "App",
  components: {
    AppNav,
    AppJumbotron,
    AppMain,
    AppMain2,
    AppMain3,
    AppMain4,
    AppJumbotron2,
    AppMain6,
  },
  mounted() {
    AOS.init();
  },
};
</script>

<style lang="scss">
@import "./style/generals.scss";
</style>
