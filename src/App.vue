<template>
  <div class="lg:px-[8rem] px-5 pt-12">
    <div class="main min-h-[100dvh]">
      <headerSection />
       <hero />
    </div>
   <!-- <headerSection />
   <hero /> -->
   <partners />
   <whyChooseClearLink />
  </div>
  <testimonial />
  <Faqs />
  <getStarted />
  <footerSection />


</template>
<script setup>
import headerSection from './components/headerSection.vue';
import hero from './components/hero.vue';
import partners from './components/partners.vue';
import whyChooseClearLink from './components/whyChooseClearLink.vue';
import testimonial from './components/testimonial.vue';
import Faqs from './components/Faqs.vue';
import getStarted from './components/getStarted.vue';
import footerSection from './components/footerSection.vue';

</script>
<style>
  *{
    font-family: 'Inter', sans-serif;
  }
  .main{
    background-image: url('@/assets/Background.png');
    /* height:100dvh; */
  }
</style>