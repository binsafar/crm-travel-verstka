<template>
  <div>
    <div class="container">
      <MainSection/>
    </div>
    <CrmBannerSection/>
    <div class="container"></div>
  </div>
</template>

<script setup>
import CrmBannerSection from "./components/sections/CrmBannerSection.vue";
import MainSection from "./components/sections/MainSection.vue";
</script>

<style>
@import "assets/styles/main.css";
</style>