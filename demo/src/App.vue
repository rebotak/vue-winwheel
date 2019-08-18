<template>
  <div id="app">
    <vue-winwheel :segments="options" />
  </div>
</template>

<script>
import VueWinwheel from "vue-winwheel/vue-winwheel";

export default {
  name: "app",
  components: {
    VueWinwheel
  },
  data() {
    return {
      options: [
        {
          textFillStyle: "#fff",
          fillStyle: "#000",
          text: "Prize 1"
        },
        {
          textFillStyle: "#000",
          fillStyle: "#fadede",
          text: "Prize 2"
        },
        {
          textFillStyle: "#fff",
          fillStyle: "#000",
          text: "Prize 3"
        },
        {
          textFillStyle: "#000",
          fillStyle: "#fadede",
          text: "Prize 4"
        },
        {
          textFillStyle: "#fff",
          fillStyle: "#000",
          text: "Prize 5"
        },
        {
          textFillStyle: "#000",
          fillStyle: "#fadede",
          text: "Prize 6"
        },
        {
          textFillStyle: "#fff",
          fillStyle: "#000",
          text: "Prize 7"
        },
        {
          textFillStyle: "#000",
          fillStyle: "#fadede",
          text: "Prize 8"
        }
      ]
    };
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
