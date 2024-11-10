<script setup>
import { ref, onMounted } from "vue";
</script>

<template>
    <div class="footer">
            <div class="f-news">
                <div class="container">
                    <div class="fn-title">
                    Join our newsletter to keep up to date with us!
                </div>
                </div>
                    <div class="fn-entry">
                        <div class="container">
                            <div class="email-wr">
                                <input type="email" class="fn-email" placeholder="someone@gmail.com">
                            </div>
                        </div>
                        <div class="container">
                            <button class="subscribe">Subscribe</button>
                        </div>
                    </div>
            </div>
        <div class="f-ct">
            <div class="f-inc">@2024 Wrenix Inc. All rights reserved.</div>
        </div>
    </div>
</template>

<style>
@import '../styles/Common.css';
@import '../styles/Footer.css';
</style>