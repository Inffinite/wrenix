<script setup>
import { routerViewLocationKey } from 'vue-router';
// import Circle from '../components/icons/Circle.vue';
import Nav from '../components/Nav.vue';
import Landing from '../components/Landing.vue';
import Reviews from '../components/Reviews.vue';
// import Services from '../components/Services.vue';
import Footer from '../components/Footer.vue';
import Faq from '../components/Faq.vue';
import About from '../components/About.vue';
// import Dev from '../components/Dev.vue';
import Process from '../components/Process.vue';

</script>

<template>
  <main>
    <div class="home">
      <Nav />
      <Landing />
      <About/>
      
      <Reviews />
      <Process />
      <Faq/>
      <Footer />
      <!-- <Dev /> -->
      <!-- <Services /> -->
      
    </div>
  </main>
</template>

<style>
@import '../styles/HomeView.css';
@import '../styles/Common.css';
</style>
