
<script setup>
import { Icon } from '@iconify/vue';
import { ref } from 'vue';
const toggleNav = ref(false);
</script>
<template>
    <header class="sticky top-0 bg-amber-100 z-50">
        <nav class="flex justify-between max-w-[1400px] mx-auto py-4 sm:py-2 px-4 items-center">
            <div class="logo flex gap-3 sm:gap-6 items-center text-primary">
                <img class="size-10 sm:size-16 mix-blend-darken" src="/src/assets/logo 2.jpeg" alt="">
                <h2 class="font-bold text-xl sm:text-2xl">Little Angel School</h2>
            </div>
            <div class="links flex gap-6" @click="toggleNav = false" :class="{'open':toggleNav}">
                <a href="#">Home</a>
                <a href="#about">About Us</a>
                <a href="#gallery">Gallery</a>
                <a href="#admission">Admission</a>
                <a href="#contact">Contact Us</a>
            </div>
            <Icon v-if="!toggleNav" icon="fa6-solid:bars" class="text-2xl md:hidden" @click="toggleNav = true" />
            <Icon v-else icon="iconamoon:sign-times-bold" class="text-4xl md:hidden" @click="toggleNav = false" />
        </nav>
    </header>
</template>

<style>
@media screen and (max-width:768px) {
    .links {
        position: fixed;
        height: 100%;
        width: 280px;
        top: 0;
        left: 0;
        flex-direction: column;
        @apply bg-amber-100 p-6 duration-100 -translate-x-full;
        box-shadow: 4px 0 8px rgba(0, 0, 0, 0.1);       
    }

    .links.open {
        @apply translate-x-0;
    }
}
</style>