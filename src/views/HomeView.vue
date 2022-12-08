<script setup>
import { routerViewLocationKey } from 'vue-router';
import Circle from '../components/icons/Circle.vue';
import Nav from '../components/Nav.vue';
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

<!-- Watch Anon again -->

<template>
  <main>
    <div class="home">
      <Nav />
      <div class="circ1">
        <Circle dimensions="200" />
        <Circle dimensions="200" />
      </div>
      <div class="home-blur">
        <div class="landing">
          <div class="container">
            <div>
              <!-- <div class="container">
                <canvas id="canvas" width="1000" height="300"></canvas>
              </div> -->
              <div class="container">
                <img src="assets/squigly-line.png" alt="" class="w-image">
              </div>
              <div class="w-title">WELCOME TO</div>
              <div class="container">
                <img class="w-name" src="../assets/wrenix.svg" alt="">
              </div>
              <div class="w-subtitle">DESIGN AGENCY</div>
            </div>
          </div>

          <div class="container">
            <div class="l-desc">
              We are a team of professional <span>Designers</span> and <span>Developers</span> in the industry.
            </div>
          </div>

          <div class="container">
            <button style="margin-top: 30px;" class="hire-btn">Lets talk</button>
          </div>
        </div>
      </div>
    </div>
  </main>
</template>

<style>
@import '../styles/HomeView.css';
@import '../styles/Common.css';
</style>
