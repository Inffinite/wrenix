<script setup>
import { ref } from "vue";
const reviews = ref(
    [
        {
            "id": 1,
            "review": "Fantastic service! They brought our vision to life with a sleek, intuitive app. Ongoing support after launch has been excellent. Highly recommend them!",
            "username": "Esther",
            "place": "Google Play Store",
        },
        {
            "id": 2,
            "review": "Great experience! The team is professional, delivers on time, and provides excellent post-launch support. The app is user-friendly, and they truly understand our needs.",
            "username": "John the Ripper",
            "place": "Google Play Store",
        },
        {
            "id": 3,
            "review": "I love your dedication to simple yet functional interfaces.",
            "username": "Mrs Grinch",
            "place": "Google Play Store",
        },
    ]
);
</script>

<template>
    <main>
        <div class="reviews">
            <div class="rv-content">
                <div class="rv-title">
                    <span class="purple">Satisfied Customers</span><br>Are Our Best Ads
                </div>
                <div class="rvc-grid">
                    <div v-for="review in reviews" :key="review.id" class="review-card">
                    <div class="container">
                        <svg class="rvc-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32" xml:space="preserve"><path d="M13 11c.6 0 1-.4 1-1s-.4-1-1-1c-5 0-9 4-9 9 0 2.8 2.2 5 5 5s5-2.2 5-5-2.2-5-5-5c-.3 0-.7 0-1 .1 1.3-1.3 3-2.1 5-2.1zM23 13c-.3 0-.7 0-1 .1 1.3-1.3 3-2.1 5-2.1.6 0 1-.4 1-1s-.4-1-1-1c-5 0-9 4-9 9 0 2.8 2.2 5 5 5s5-2.2 5-5-2.2-5-5-5z"/></svg>
                    </div>
                    <div class="rvc-review">
                        {{review.review}}
                    </div>
                    <div class="rvc-name">
                        {{review.username}} - {{review.place}}
                    </div>
                </div>
                </div>
            </div>
        </div>
    </main>
</template>

<style>
@import '../styles/Reviews.css';
@import '../styles/Common.css';
</style>