<template>
    <div class="flex justify-center gap-3 mt-6">
        <button v-for="icon of icons">
            <img :src="icon.img" :alt="icon.alt">
        </button>
    </div>
</template>
<script setup>
import { ref } from 'vue';
import mic from '../assets/mic.png'
import settings from '../assets/settings.png'
import vid from '../assets/vid.png'
import tv from '../assets/tv.png'
import message from '../assets/message.png'
import emoji from '../assets/emoji.png'
    const icons = ref([
        {
            img: mic,
            alt:'mic'
        },
        {
            img: vid,
            alt:'vid'
        },
        {
            img: tv,
            alt:'tv'
        },
        {
            img: emoji,
            alt:'emoji'
        },
        {
            img: message,
            alt:'message'
        },
        {
            img: settings,
            alt: 'settings'
        }
    ])
</script>