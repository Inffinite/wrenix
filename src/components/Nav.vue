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
            <div class="nav-ct">
                <img src="../assets/wrenix-nav-logo.svg" alt="" class="nav-logo">
            <div class="container nope">
                <ul class="nope">Home</ul>
                <ul class="nope">Reviews</ul>
                <ul class="nope">Contact</ul>
            </div>
            <button class="n-btn nope">
                Talk to us
                <svg class="n-btn-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor">
                <path fill-rule="evenodd" d="M12 2.25c-2.429 0-4.817.178-7.152.521C2.87 3.061 1.5 4.795 1.5 6.741v6.018c0 1.946 1.37 3.68 3.348 3.97.877.129 1.761.234 2.652.316V21a.75.75 0 0 0 1.28.53l4.184-4.183a.39.39 0 0 1 .266-.112c2.006-.05 3.982-.22 5.922-.506 1.978-.29 3.348-2.023 3.348-3.97V6.741c0-1.947-1.37-3.68-3.348-3.97A49.145 49.145 0 0 0 12 2.25ZM8.25 8.625a1.125 1.125 0 1 0 0 2.25 1.125 1.125 0 0 0 0-2.25Zm2.625 1.125a1.125 1.125 0 1 1 2.25 0 1.125 1.125 0 0 1-2.25 0Zm4.875-1.125a1.125 1.125 0 1 0 0 2.25 1.125 1.125 0 0 0 0-2.25Z" clip-rule="evenodd" />
                </svg>

            </button>
            </div>
        </div>
    </main>
</template>

<style>
@import '../styles/Common.css';
@import '../styles/Nav.css';
</style>