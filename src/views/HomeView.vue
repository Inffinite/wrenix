<script setup>
import { routerViewLocationKey } from 'vue-router';
import Circle from '../components/icons/Circle.vue';
import Nav from '../components/Nav.vue';
import Landing from '../components/Landing.vue';
import Reviews from '../components/Reviews.vue';
import Services from '../components/Services.vue';
import Footer from '../components/Footer.vue';
import Dev from '../components/Dev.vue';

</script>

<template>
  <main>
    <div class="home">
      <Nav />
      <Landing />
      <Footer />
      <!-- <Dev /> -->
      <!-- <Services /> -->
      <!-- <Reviews /> -->
    </div>
  </main>
</template>

<style>
@import '../styles/HomeView.css';
@import '../styles/Common.css';
</style>
