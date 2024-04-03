<template>
  <main>
    <div class="container">
      <Header/>
      <MainSection/>
    </div>

    <CrmBannerSection/>

    <div class="container">
      <FaqSection/>
      <SendApplicationSection/>
    </div>

    <OfferedServicesSection/>

    <div class="container">
      <HowWorksSection/>
      <Plans/>
      <TryDemoSection/>
    </div>

    <Footer/>
  </main>
</template>

<script setup>
import CrmBannerSection from "./components/sections/CrmBannerSection.vue";
import MainSection from "./components/sections/MainSection.vue";
import SendApplicationSection from "./components/sections/SendApplicationSection.vue";
import TryDemoSection from "./components/sections/TryDemoSection.vue";
import Header from "./components/Header.vue";
import FaqSection from "./components/sections/FaqSection.vue";
import OfferedServicesSection from "./components/OfferedServicesSection.vue";
import HowWorksSection from "./components/sections/HowWorksSection.vue";
import Footer from "./components/Footer.vue";
import Plans from "./components/sections/Plans.vue";
</script>
