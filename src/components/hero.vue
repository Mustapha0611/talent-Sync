<template>
  <div class="flex flex-col lg:flex-row mt-32 h-auto lg:min-h-[60vh]">
    <section class=" px-5 flex-1" data-aos="zoom-in" data-aos-delay="80">
      <h1 class="md:text-[50px] text-3xl leading-[1.3] font-semibold max-w-[600px]" >
        Uniting the world, one video call at a time
      </h1>
      <p class="w-3/4 mt-6">
        Experience the future of communication with ClearLink – where
        crystal-clear video conferencing meets unparalleled simplicity.
      </p>
      <div class="my-12 flex gap-4 flex-col md:flex-row">
        <button class="py-2 px-5 text-white bg-blue-700 rounded-3xl text-xs md:text-lg" aria-label="Start free trial">Start your free trail</button>
        <button class="flex items-center py-2 px-5 text-gray-900 text-xs md:text-lg rounded-3xl gap-2" aria-label="Ai assistant">
          <img src="../assets/robot.png" alt="robot" /><span
            >Discover AI assistant</span
          >
        </button>
      </div>
      <span>
        <img src="../assets/reviews.png" alt="reviews" />
      </span>
    </section>
    <section class="bg-blue-100 p-8 mt-10 lg:my-0 max-h-[470px] rounded-xl border-2 border-blue-200 shadow-xl">
      
        <div class="grid grid-cols-3 gap-4 ">
          <div class="" v-for="profile of profiles">
            <img :src="profile.img" :alt="profile.alt" />
          </div>
        
      </div>
      <btnsFLex />
    </section>
  </div>
</template>
<script setup>
import { ref } from "vue";
import old from "../assets/old.png";
import blackwoman from "../assets/blackwoman.png";
import white from "../assets/white.png";
import arab from "../assets/arab.png";
import dude from "../assets/dude.png";
import lady from "../assets/lady.png";
import btnsFLex from "./btnsFLex.vue";
const profiles = ref([
  {
    img: old,
    alt:'old'
  },
  {
    img: blackwoman,
    alt:'black'
    
  },
  {
    img: white,
    alt:'white'
  },
  {
    img: arab,
    alt:'arab'
  },
  {
    img: dude,
    alt:'dude'
  },
  {
    img: lady,
    alt:'lady'
  },
]);

</script>
