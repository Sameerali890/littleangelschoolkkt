<script setup>
import { Icon } from "@iconify/vue";
</script>

<template>
    <div id="contact" class="bg-primary border-t border-amber-100">
        <div class="grid sm:grid-cols-2 py-16 max-w-[1400px] mx-auto">
            <div class="px-6 max-sm:mb-8">
                <iframe
                    src="https://www.google.com/maps/embed?pb=!1m14!1m8!1m3!1d14387.971823662005!2d82.9124961!3d25.6383593!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x3991d2d6a89661f1%3A0xb7e15e926c4e6aec!2sLittle%20Angel%20School!5e0!3m2!1sen!2sin!4v1711015355157!5m2!1sen!2sin" height="300" style="border: 0" allowfullscreen="" loading="lazy"
                    referrerpolicy="no-referrer-when-downgrade"></iframe>
            </div>
            <div class="grid place-items-center">
                <div class="grid content-center text-amber-50">
                    <h1 class="text-4xl font-bold mb-4">Contact Us</h1>
                    <div class="sm:text-lg">
                        <p class="leading-[2.1]">Little Angel School, Kerakat, Jaunpur</p>
                        <p class="">Uttar Paradesh (India)</p>
                    </div>
                    <a class="sm:text-lg mt-2" href="tel:+919450083483" target="_blank">+91-9450083483</a>
                    <a class="sm:text-lg mt-1" href="mailto:littleangelschoolkkt@gmail.com"
                        target="_blank">littleangelschoolkkt@gmail.com</a>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
 iframe {
    width: min(600px, 100%);
 }
</style>