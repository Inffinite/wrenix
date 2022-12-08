<script setup>
import ReviewCard from "./ReviewCard.vue";
</script>

<template>
    <main>
        <div class="reviews">
            <div class="r-title">
                Our happy customers
            </div>

            <ReviewCard name="Person" workplace="Chum Bucket"
                message="Lorem ipsum dolor sit amet, consectetur adipisicing elit. Et delectus recusandae placeat sed, ex quidem maiores dolore deserunt!" />
        </div>
    </main>
</template>

<style>
@import "../styles/Reviews.css";
@import "../styles/Common.css";
</style>