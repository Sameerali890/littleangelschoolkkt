
<script setup>
    import { Icon } from '@iconify/vue';
</script>
<template>
    <div class="grid grid-cols-2 py-20 max-w-[1400px] mx-auto">
        <div class="px-4">
            <img class="h-[400px] w-[600px] rounded-lg object-cover " src="/src/assets/cover photo2.jpg" alt="">
        </div>
        <div class="grid place-items-center">
            <div class="grid content-center max-w-xl text-primary">
                <h1 class="text-4xl font-bold mb-4">About Our School</h1>
                <p class="mb-2">We aim to provide intelligent guidance, constructive discipline and good learning to assure that education is not merely the road to earning and living but the gateway of knowledge. The first word of Quran revealed on prophet (pbuh) was <b><q>IQRA</q></b> which means <b><q>READ</q></b>. Further, in the same verse it is commanded,</p>
                <div class="mb-8">
                    <b><q>Allamal insana malam yalam</q></b>
                     - Allah taught the man that which he knew not.
                </div>
                <div class="flex gap-32">
                    <div class="achieve">
                        <div class="size-20 bg-primary text-amber-50 rounded-md grid place-items-center text-5xl">
                            <Icon icon="ph:student-bold" />
                        </div>
                        <h3 class="border-primary">1200 <Icon icon="material-symbols:add" /></h3>
                        <h2 class="font-semibold">Students</h2>
                    </div>
                    <div class="achieve">
                        <div class="size-20 bg-primary text-amber-50 rounded-md grid place-items-center text-5xl">
                            <Icon icon="flowbite:users-group-outline" />
                        </div>
                        <h3 class="border-primary">20 <Icon icon="material-symbols:add" /></h3>
                        <h2 class="font-semibold">Staffs</h2>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
    .achieve h3{
       @apply border-b-4 text-3xl pb-2 flex items-center;

    }
    .achieve h2{
        text-transform: uppercase ;
        padding-top: 8px;
    }

    .achieve{
        display: grid;
        grid-template-columns: max-content auto;
        gap: 0 16px;
    }

    .achieve > div:first-child {
        grid-row: span 3;
    }
</style>