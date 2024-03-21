<script setup>
import { Icon } from '@iconify/vue';
</script>

<template>
    <section class="grid  py-12 px-4    ">
        <div class="grid place-items-center gap-8">
            <img class="mix-blend-darken size-24" src="/src/assets/logo 2.jpeg" alt="">
            <div class="flex gap-8">
                <a href="http://">About Us</a>
                <a href="http://">Gallery</a>
                <a href="http://">Admissions</a>
                <a href="http://">Contact Us</a>
            </div>
            <div class="flex items-center gap-2">
                <icon icon="ri:facebook-box-fill" />
                <a href="http://facebook.com">Facebook</a>
                <icon class="ml-5" icon="teenyicons:instagram-outline" />
                <a href="http://instagram.com">Instagram</a>
                <icon class="ml-5" icon="octicon:mail-16" />
                <a href="mailto:littleangelschoolkkt@gmail.com" target="blank">littleangelschoolkkt@gmail.com</a>
            </div>
        </div>
    </section>
</template>