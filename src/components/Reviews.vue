<script setup>
import ReviewCard from "./ReviewCard.vue";

function openLink() {
    window.open("https://wa.link/mapl4a");
}
</script>

<template>
    <main>
        <div class="reviews">
            <div class="r-title">
                Our happy customers
            </div>

            <div class="my-reviews">
                <ReviewCard name="Jack" workplace="Philanthropist"
                    imageUrl="https://randomuser.me/api/portraits/men/50.jpg"
                    message="Delivered my work on time and within my deadline. Love it." />

                <ReviewCard name="April Graham" workplace="Artist"
                    imageUrl="https://randomuser.me/api/portraits/women/51.jpg"
                    message="Creative and delightful to work with." />

                <ReviewCard name="Lucy Lane" workplace="Technical Writer"
                    imageUrl="https://randomuser.me/api/portraits/women/36.jpg"
                    message="Decent work quality and all round customer service." />
            </div>

            
        </div>
    </main>
</template>

<style>
@import "../styles/Reviews.css";
@import "../styles/Common.css";
</style>