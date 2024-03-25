<template>
  <div>
    <div class="container">
      <MainSection/>
    </div>
    <CrmBannerSection/>
    <div class="container">
      <SendApplicationSection/>
      <TryDemoSection/>
    </div>
  </div>
</template>

<script setup>
import CrmBannerSection from "./components/sections/CrmBannerSection.vue";
import MainSection from "./components/sections/MainSection.vue";
import SendApplicationSection from "./components/sections/SendApplicationSection.vue";
import TryDemoSection from "./components/sections/TryDemoSection.vue";
</script>

<style>
@import "assets/styles/main.css";
</style>