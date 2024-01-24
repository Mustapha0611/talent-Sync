<template>
    <div class="mt-20 md:py-20 py-5 px-8" data-aos="fade-up">
        <h2 class="text-center text-gray-600 text-sm md:text-xl font-semibold">
            Join 1,500+ companies already video conferencing the ClearLink way
        </h2>
        <section class="flex justify-between items-center my-12 flex-wrap gap-4">
            <div v-for="partner of partners" >
                <img :src="partner.img" :alt="partner.alt">
            </div>
        </section>
    </div>
</template>
<script setup>
import { ref } from 'vue';
import shopify from '../assets/shopify.png'
import Coinbase from '../assets/Coinbase.png'
import Dropbox from '../assets/Dropbox.png'
import intercom from '../assets/Intercom.png'
import marvel from '../assets/marvel.png'
import auto from '../assets/auto.png'
    const partners = ref([
        {
            img: shopify,
            alt:'shopify'
        },
        {
            img: Coinbase,
            alt:'Coinbase'
        },
        {
            img: Dropbox,
            alt:'Dropbox'
        },
        {
            img: intercom,
            alt:'intercom'
        },
        {
            img: marvel,
            alt:'marvel'
        },
        {
            img: auto,
            alt: 'automatic'
        }
    ])

</script>