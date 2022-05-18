<template>
  <div id="app">
    <app-nav :datiNavbar="datiNavbar" />
    <app-jumbotron />
    <app-cards-bg />
    <app-section-cards />
    <app-jumbotron-2 />
    <app-jumbotron-cards />
    <app-playlist />

    <app-logo-cards />
    <app-jumbotron-3 />
    <app-footer :datiFooter="datiFooter" />
  </div>
</template>

<script>
import dati from "./dati.json";
import AOS from "aos";
import AppNav from "./components/1-AppNav.vue";
import AppJumbotron from "./components/2-AppJumbotron.vue";
import AppCardsBg from "./components/3-AppCards+Bg.vue";
import AppSectionCards from "./components/4-AppSectionCards.vue";
import AppJumbotronCards from "./components/6-AppJumbotronCards.vue";
import AppPlaylist from "./components/7-AppPlaylist.vue";
import AppJumbotron2 from "./components/5-AppJumbotron2.vue";
import AppLogoCards from "./components/8-AppLogoCards.vue";
import AppJumbotron3 from "./components/9-AppJumbotron3.vue";
import AppFooter from "./components/10-AppFooter.vue";

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
    AppCardsBg,
    AppSectionCards,
    AppJumbotronCards,
    AppPlaylist,
    AppJumbotron2,
    AppLogoCards,
    AppJumbotron3,
    AppFooter,
  },
  mounted() {
    AOS.init();
  },
};
</script>

<style lang="scss">
@import "./style/generals.scss";
</style>
