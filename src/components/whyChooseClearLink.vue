<template>
    <div class="md:py-20 py-5 relative">
        <h4 class="text-[18px] text-blue-700 font-semibold mb-3" data-aos="fade-right">
            The ClearLink Advantage
        </h4>
        <h5 class="md:text-5xl text-2xl text-gray-800 font-semibold mb-5" data-aos="fade-right">
            Why Choose ClearLink?
        </h5>
        <p class="max-w-[900px] text-gray-500 font-normal md:text-2xl text-xl mb-20" data-aos="fade-right" >
            In a world where connection is everything, ClearLink takes the lead. Our cutting-edge video conferencing app offers:
        </p>
        <div class="flex flex-col lg:flex-row">
            <section class="grid grid-cols-1  lg:grid-cols-2 gap-5 text-pretty mr-10">
                <div v-for="feature of features" class="mb-10 pr-5 max-w-[500px] " data-aos="zoom-in">
                    <img :src="feature.img" alt="feature" class="mb-5"/>
                    <h5 class="font-semibold text-xl text-gray-900 mb-2">{{ feature.title }}</h5>
                    <p class="text-gray-600 font-normal">{{ feature.body }}</p>
                </div>
            </section>
            <section>
                <div class="max-w-[500px] max-h-[500px]">
                    <img src="../assets/rect.png" alt="people" class="w-full h-full">
                </div>
            </section>
            
        </div>
        <div class="absolute lg:right-[12%] lg:top-28 right-[14%] top-[75rem]">
            <img src="../assets/arrow.png" alt="arrow down">
        </div>
    </div>
</template>
<script setup>
import { ref } from 'vue';
import vid from '../assets/zap.png'
import recording from '../assets/recording.png'
import calendar from '../assets/calendar.png'
import lock from '../assets/lock.png'

    const features = ref([
        {
            img:vid,
            title:"Crystal-clear HD video",
            body:"No more pixelation or blurriness – just stunning, lifelike clarity that brings your team closer in meetings."
        },
        {
            img:recording,
            title:"Noise-canceling audio",
            body:"Say goodbye to distractions with our advanced audio tech for crisp, interruption-free conversations."
        },
        {
            img:calendar,
            title:"Scheduling made easy",
            body:"Streamline your agenda with ClearLink's intuitive scheduling. Set up meetings, send invitations, and receive reminders in one place."
        },
        {
            img:lock,
            title:"Bank-grade security",
            body:"Your privacy is our priority with bank-grade security protocols safeguarding your meetings and data from unwanted intruders."
        },
    ])
</script>