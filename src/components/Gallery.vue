<script setup>
import { Icon } from '@iconify/vue';
import { ref } from 'vue'
const currentImage = ref("");
</script>

<template>
    <section id="gallery" class="gap-4 sm:gap-8 max-w-[1400px] mx-auto pt-4 pb-8 lg:py-16">
        <div class="heading">Gallery</div>
        <img @click="currentImage = $event.target.src" v-for="image in 6" :src="'/images/'+image+'.jpg'" alt="">
    </section>

    <div v-if="currentImage" class="model max-sm:p-4"  @click="currentImage=''">
        <Icon @click="currentImage=''" icon="humbleicons:times" class="absolute top-6 right-6 text-white text-4xl cursor-pointer hover:text-red-500" />
        <img @click="$event.stopPropagation()" :src="currentImage">
    </div>
</template>

<style scoped>
section {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(320px, 1fr));
    padding-inline: 16px;
}
    section img {
        @apply  rounded-md hover:scale-105 duration-300;
        aspect-ratio: 4/3;
        object-fit: cover;
        border: 8px solid white;
        box-shadow: 0 0 8px 1px rgba(0, 0, 0, 0.2);
        
    }

    .heading {
        grid-column: 1/-1;
        text-align: center;
        @apply text-4xl mb-4 font-[700];
        color: var(--primary);
    }

    .model {
        @apply fixed inset-0 bg-black/90 grid place-items-center ;
        z-index: 51;

    }

    .model img {
        width: min(100%,1000px);
        aspect-ratio: 7/5;
        margin: 0 auto;
    }
</style>