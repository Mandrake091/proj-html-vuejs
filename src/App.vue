<template>
  <div id="app">
    <app-nav :datiNavbar="datiNavbar" />
    <app-jumbotron/>
  </div>
</template>

<script>
import dati from "./dati.json";
import AOS from "aos";
import AppNav from "./components/AppNav.vue";
import AppJumbotron from "./components/AppJumbotron.vue";

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
  },
  methods: {},
  mounted() {
    AOS.init();
  },
};
</script>

<style lang="scss">
@import "./style/generals.scss";

#app {
}
</style>
