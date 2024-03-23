<script setup>
import { Icon } from '@iconify/vue';
</script>

<template>
    <section class="grid  py-12 px-4    ">
        <div class="grid place-items-center gap-8">
            <img class="mix-blend-darken size-24" src="/src/assets/logo 2.jpeg" alt="">
            <div class="flex gap-[16px_32px] max-sm:flex-wrap justify-center">
                <a href="#">Home</a>
                <a href="#about">About Us</a>
                <a href="#gallery">Gallery</a>
                <a href="#admission">Admissions</a>
                <a href="#contact">Contact Us</a>
            </div>
            <div class="flex items-center gap-4 sm:gap-12 max-sm:flex-wrap justify-center">
                <div class="flex items-center gap-2">
                    <icon icon="ri:facebook-box-fill" />
                    <a href="https://www.facebook.com/littleangelschoolkkt">Facebook</a>
                </div>
                <div class="flex items-center gap-2">
                    <icon icon="teenyicons:instagram-outline" />
                    <a href="http://instagram.com">Instagram</a>
                </div>
                <div class="flex items-center gap-2">
                    <icon icon="octicon:mail-16" />
                    <a href="mailto:littleangelschoolkkt@gmail.com" target="blank">littleangelschoolkkt@gmail.com</a>
                </div>
            </div>
        </div>
    </section>
</template>