<script setup>
import NavBar from "./components/NavBar.vue"
import Core from "./components/Core.vue"
import Info from "./components/Info.vue"
import OtherSites from "./components/OtherSites.vue"
import Footer from "./components/Footer.vue"
</script>

<template>
  <div class="col-12 m-auto">
    <NavBar/>
    <Core/>
    <Info/>
    <OtherSites/>
    <Footer/>
  </div>
</template>

<style lang="scss">
@use "./style/main.scss" as *;



</style>