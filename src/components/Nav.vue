<script setup>
import { ref, onMounted } from "vue";

// onMounted(() => {
//     console.log(mobileNavStatus.value)
// })

const mobileNavStatus = ref(false);
const navClass = ref("m-nav");

function mobileNav() {
    switch (mobileNavStatus.value) {
        case false:
            navClass.value = "m-nav-open"
            mobileNavStatus.value = true
            break;

        case true:
            navClass.value = "m-nav"
            mobileNavStatus.value = false
            break

        default:
            break;
    }
}
</script>

<template>
    <main>
        <div>
            <div :class="navClass">
                <div class="n-logo">
                    <img class="n-l" src="../assets/wrenix.svg" alt="" />
                </div>
                <!-- <svg @click="mobileNav" v-if="mobileNavStatus == false" class="n-icon"
                    xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                    stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M3.75 9h16.5m-16.5 6.75h16.5" />
                </svg> -->

                <!-- <svg @click="mobileNav" v-if="mobileNavStatus == true" xmlns="http://www.w3.org/2000/svg" fill="none"
                    viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="n-icon">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12" />
                </svg> -->

                <div v-if="mobileNavStatus == true" class="m-menu-items">
                    <div class="m-item">
                        Resources
                    </div>
                    <div class="m-item">
                        Services
                    </div>
                    <div class="m-item">
                        About
                    </div>
                    <div class="m-item">
                        Contact
                    </div>
                </div>
            </div>

            <div class="d-nav">
                <div class="n-logo">
                    <img class="n-l" src="../assets/wrenix.svg" alt="" />
                </div>
                <!-- <div class="n-item">Resources</div>
                <div class="n-item">Services</div>
                <div class="n-item">About</div>
                <div class="n-item">Contact</div> -->
            </div>
        </div>
    </main>
</template>

<style>
@import '../styles/Common.css';
@import '../styles/Nav.css';
</style>