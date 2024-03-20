<script setup>
    import { Icon } from '@iconify/vue';
</script>

<template>
    <section class="grid grid-cols-3 justify-center place-items-center  mx-auto">
        <div class="left">
            <div class="first grid items-center">
                <img class="mix-blend-darken size-16 mt-4" src="/src/assets/logo 2.jpeg" alt="">
                <div class="mt-3">Little Angel School</div>
                <div>Kerakat, Jaunpur</div>
                <div>Uttar Paradesh (India)</div>
            </div>
            <div class="sec flex  items-center  gap-2 mt-5">
                <icon icon="material-symbols:call-outline"/>
                <a href="tel:+">+91-9450083483</a>
            </div>
            <div class="flex  items-center gap-2">
                <icon icon="material-symbols:mail-outline"/>
                <a href="mailto:littleangelschoolkkt@gmail.com">littleangelschoolkkt@gmail.com</a>
            </div>
            
        </div>
        <div class="right">
            <h1>About US</h1>
            <h1>Gallery</h1>
            <h1>Admission</h1>
        </div>
        <div class="links grid">
            <a href="http://https://www.facebook.com/littleangelschoolkkt/">Facebook</a>
            <a href="">Youtube</a>
            <a href="">Twitter</a>
        </div>
    </section>
</template>