<template>
  <div id="app">
    <main-tar-bar></main-tar-bar>
    <router-view></router-view>
  </div>
</template>

<script>
import MainTarBar from "components/conters/maintarbar/MainTarBar";


export default {
  name: 'App',
  components: {
    MainTarBar

  }
}
</script>

<style>
@import "assets/css/base.css";
</style>
