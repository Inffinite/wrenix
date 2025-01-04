<script setup>
import Circle from '../components/icons/Circle.vue';
// import { Rive, Layout } from "@rive-app/canvas";
import { ref, onMounted } from "vue";

onMounted(() => {
  // new Rive({
  //   src: "./birdy.riv",
  //   canvas: document.getElementById('canvas'),
  //   layout: new Layout({ fit: 'contain', alignment: 'center' }),
  //   autoplay: true,
  // });
})

function openLink() {
    window.open("https://wa.link/mapl4a");
}
</script>

<template>
    <main>
        <div class="landing">
          <div class="container">
            <div class="l-title">
              We build Interactive <span class="glow">Mobile Experiences.</span>
            </div>
          </div>
          <div class="container">
            <div class="l-subtitle">
              We're pushing the boundaries of mobile technology to deliver extraordinary experiences.
            </div>
          </div>
          <div class="container">
            <button class="l-btn">
              Work With Us
            </button>
          </div>
        </div>
    </main>
</template>

<style>
@import '../styles/Common.css';
@import '../styles/Landing.css';
</style>