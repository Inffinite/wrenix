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
        <div class="nav">
            <img src="../assets/wrenix-nav-logo.svg" alt="" class="nav-logo">
        </div>
    </main>
</template>

<style>
@import '../styles/Common.css';
@import '../styles/Nav.css';
</style>