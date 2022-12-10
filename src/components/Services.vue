<script setup>
import ServiceCard from "./ServiceCard.vue";
const ui = ["Website interfaces", "IOT device interfaces", "Mobile/Desktop interfaces"]
const software = ["Cloud applications", "Mobile applications", "Desktop applications"]
const graphic = ["Publications", "Logos", "Posters"]
</script>

<template>
    <main>
        <div class="services">
            <div class="s-title">Our Services</div>

            <div class="s-card-wr">
                <ServiceCard iconType="1" title="Software Development" :options=software />
                <ServiceCard iconType="2" title="UI/UX Design" :options=ui />
                <ServiceCard iconType="3" title="Graphic Design" :options=graphic />
            </div>
        </div>
    </main>
</template>

<style>
@import "../styles/Services.css";
@import "../styles/Common.css";
</style>