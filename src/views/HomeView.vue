<script setup>
import { routerViewLocationKey } from 'vue-router';
import Circle from '../components/icons/Circle.vue';
import Nav from '../components/Nav.vue';
import Landing from '../components/Landing.vue';
// import { Rive, Layout } from "@rive-app/canvas";
import { ref, onMounted } from "vue";


// onMounted(() => {
//   new Rive({
//     src: "assets/birdy.riv",
//     canvas: document.getElementById('canvas'),
//     layout: new Layout({ fit: 'contain', alignment: 'center' }),
//     autoplay: true,
//   });
// })
</script>

<template>
  <main>
    <div class="home">
      <Nav />
      <Landing />
    </div>
  </main>
</template>

<style>
@import '../styles/HomeView.css';
@import '../styles/Common.css';
</style>
