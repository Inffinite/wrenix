<script setup>
import { ref } from 'vue';
import axios from 'axios';
import { useRouter } from 'vue-router';

const router = useRouter();

const name = ref("");
const buttonMessage = ref('Send')
const error = ref(false);
const phoneNumber = ref("");
const message = ref("");

async function handleSubmit(){
    error.value = false
    buttonMessage.value = 'Loading...'
    console.log(name.value + phoneNumber.value + message.value)

    await axios.post('https://server.wrenix.org/messages', {
        name: name.value,
        phone: phoneNumber.value,
        message: message.value,
    })
    .then((res) => {
        router.push('/success')
    })
    .catch((e) => {
        buttonMessage.value = 'Sends'
        console.log(e);
        error.value = true
    })
}

</script>

<template>
    <main>
        <div class="message">
            <div class="ms-ct">
                <div class="ms-title">Contact us</div>
                <div class="ms-subtitle">We will get back to you soon</div>

                <div class="ms-form">
                    <form @submit.prevent="handleSubmit">
                        <div class="ms-label">Name</div>
                        <div class="ms-box">
                            <input type="text" required v-model="name" class="name" placeholder="Rupert Winkles">
                        </div>

                        <div class="ms-label">Phone Number</div>
                        <div class="ms-box">
                            <input type="number" required v-model="phoneNumber" class="name" placeholder="254749087865">
                        </div>
                        
                        <div class="ms-label">Message</div>
                        <div class="ms-box">
                            <textarea class="name" required v-model="message" rows="5" placeholder="I like onions..."></textarea>
                        </div>
                        
                        <div v-if="error" class="ms-error">
                            Failed. Check your internet connection or try again later.
                        </div>
                        <div class="ms-btn-wr"><button class="ms-btn">{{ buttonMessage }}</button></div>
                </form>
                </div>
            </div>
        </div>
    </main>
</template>

<style>
@import '../styles/Common.css';
@import '../styles/Message.css';
</style>