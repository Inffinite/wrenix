<script setup>
import { useRouter } from 'vue-router';

const router = useRouter();

function homepage(){
    router.push('/');
}
</script>

<template>
    <main>
        <div class="success">
            <div class="sc-ct">
                <div class="sc-title">
                    Sent
                </div>
                <div class="sc-subtitle">
                    <span class="purple">Your message has been received.</span> We value your inquiry and will respond to you as soon as possible. We look forward to connecting with you soon.
                </div>
                <div class="sc-home-wr">
                    <button @click="homepage()" class="sc-home">Back to homepage</button>
                </div>
            </div>
        </div>
    </main>
</template>

<style>
@import '../styles/Common.css';
@import '../styles/Success.css';
</style>