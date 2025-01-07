<script setup>
import Circle from '../components/icons/Circle.vue';
// import { Rive, Layout } from "@rive-app/canvas";
import { ref, onMounted } from "vue";
import { useRouter } from 'vue-router';

const router = useRouter();

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

function messages(){
  router.push('/message')
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
            <button @click="messages()" class="l-btn">
              Talk To Us
            </button>
          </div>
        </div>
    </main>
</template>

<style>
@import '../styles/Common.css';
@import '../styles/Landing.css';
</style>