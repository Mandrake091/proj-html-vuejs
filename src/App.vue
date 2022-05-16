<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
   

  </div>
</template>

<script>
import AOS from "aos"
import HelloWorld from './components/HelloWorld.vue'

export default {
  data(){
    return{

    }

  },
  name: 'App',
  components: {
    HelloWorld
  },
  methods:{

  },
  mounted(){
    AOS.init();
  }
}
</script>

<style lang="scss">
@import "./style/generals.scss";


#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
