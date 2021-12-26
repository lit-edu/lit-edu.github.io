<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <div class="head-bg-wrapper">
      <h1 class="title">洛阳理工学院<br />新媒体矩阵</h1>
      <!-- <img class="head-bg" src="@/assets/bg.jpg" fluid alt="bg"/>  -->
    </div>
    <center>
      <div class="block-list">
        <MyBlock />
        <MyBlock />
        <MyBlock />
        <MyBlock />
        <MyBlock />
        <MyBlock />
        <MyBlock />
        <MyBlock />
        <MyBlock />
        <MyBlock />
        <MyBlock />
        <MyBlock />
      </div>
    </center>
  </div>
  <!-- <div class="test">test</div> -->

  <!-- <b-img v-bind="mainProps" rounded alt="Rounded image"></b-img> -->
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'

import MyBlock from "./components/MyBlock.vue";

import Vue from "vue";
import { BootstrapVue, IconsPlugin } from "bootstrap-vue";
import "bootstrap/dist/css/bootstrap.css";
import "bootstrap-vue/dist/bootstrap-vue.css";
// Make BootstrapVue available throughout your project
Vue.use(BootstrapVue);
// Optionally install the BootstrapVue icon components plugin
Vue.use(IconsPlugin);

export default {
  name: "App",
  components: {
    // HelloWorld,
    MyBlock,
  },
  data() {
    return {
      mainProps: { blank: true, blankColor: "#777", width: 75, height: 75 },
    };
  },
};
</script>

<style>
#app {
  font-family: Source Sans Pro, Helvetica;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  margin-top: 0px;
}
body {
  background: #eef0ff;
}
.test {
  background-color: blueviolet;
  width: 100%;
  height: 600px;
}
.title {
  font-family: Source Sans Pro;
  font-style: normal;
  font-size: 37px;
  font-weight: 900;
  text-align: center;
  color: rgb(255, 255, 255);
}
.head-bg-wrapper {
  background-image: linear-gradient(
      99.98deg,
      rgba(48, 63, 159, 0.64) 0%,
      rgba(121, 134, 203, 0.46) 100%
    ),
    url("./assets/bg.jpg");
  background-position-y: 50%;
  background-size: 100%;
  display: flex;
  position: block;
  width: 100%;
  height: 170px;
  background-color: aqua;
  align-items: center;
  justify-content: center;
}
.head-bg {
  width: auto;
  height: 170px;
}
.block-list {
  margin: 16px 0px;
  max-width: 370px;
  flex-wrap: wrap;
  display: flex;
  justify-content: center;
}
</style>
