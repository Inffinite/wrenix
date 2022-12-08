<script setup>
import Circle from '../components/icons/Circle.vue';
</script>

<template>
    <main>
        <div class="landing">
            <div class="container">
                <div>
                    <!-- <div class="container">
                        <canvas id="canvas" width="1000" height="300"></canvas>
                      </div> -->
                    <div class="circ1">
                        <Circle />
                        <div class="container">
                            <img src="assets/squigly-line.png" alt="" class="w-image">
                        </div>
                        <Circle />
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
                <button style="margin-top: 40px;" class="hire-btn">Lets talk</button>
            </div>
        </div>
    </main>
</template>

<style>
@import '../styles/Common.css';
@import '../styles/Landing.css';
</style>