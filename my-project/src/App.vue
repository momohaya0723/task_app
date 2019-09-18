<template>
  <div id="app">
    <myheader></myheader>
    <img src="./assets/logo.png">
    <router-view/>
    <myfooter></myfooter>
  </div>
</template>

<script>
import 'bootstrap/dist/css/bootstrap.css'
import 'bootstrap-vue/dist/bootstrap-vue.css'

import myheader from './components/myheader'
import myfooter from './components/myfooter'

export default {
  name: 'App',
  components: {
    myheader,
    myfooter
  },
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
