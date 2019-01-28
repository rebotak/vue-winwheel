<template>
  <div id="app">
    <vue-winwheel
      :segments="options"
      :wheelSize="wheelSize"
      :pageTitle="pageTitle"
      :lineWidth="lineWidth"
      :btnColor="btnColor"
      :btnText="btnText"
      :spinSound="spinSound"
      :customSpinSound="customSpinSound"
    />
  </div>
</template>

<script>
import VueWinwheel from './VueWinwheel.vue'

export default {
  name: 'app',
  components: {
    VueWinwheel
  },
  data(){
    return{
      pageTitle       : "Vue-Wheel",
      wheelSize       : 400,
      btnColor        : "",
      btnText         : "",
      lineWidth       : 3,
      spinSound       : true,
      customSpinSound : "",
      options         :[
					{
						textFillStyle: '#fff',
						fillStyle: '#000',
						text:'Prize 1',
            desc: "Description 1"
					},
					{
						textFillStyle: '#000',
						fillStyle: '#fadede',
						text:'Prize 2',
            desc: "Description 2"
					},
					{
						textFillStyle: '#fff',
						fillStyle: '#000',
						text:'Prize 3',
            desc: "Description 3"
					},
					{
						textFillStyle: '#000',
						fillStyle: '#fadede',
						text:'Prize 4',
            desc: "Description 4"
					},
					{
						textFillStyle: '#fff',
						fillStyle: '#000',
						text:'Prize 5',
            desc: "Description 5"
					},
					{
						textFillStyle: '#000',
						fillStyle: '#fadede',
						text:'Prize 6',
            desc: "Description 6"
					},
					{
						textFillStyle: '#fff',
						fillStyle: '#000',
						text:'Prize 7',
            desc: "Description 7"
					},
					{
						textFillStyle: '#000',
						fillStyle: '#fadede',
						text:'Prize 8',
            desc: "Description 8"
					}
				]
    }
  }
}
</script>

<style>
#app {
	font-family: 'Avenir', Helvetica, Arial, sans-serif;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
	text-align: center;
	color: #2c3e50;
	margin-top: 60px;
}
</style>
