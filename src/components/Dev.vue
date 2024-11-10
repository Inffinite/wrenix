<script setup>
    function openNewTab() {
      window.open('https://trex-runner.com/', '_blank');
    }
</script>

<template>
    <div class="dev">
        <div class="dev-ct">
            <img src="../assets/wrenix-logo.png" alt="Logo" class="logo-dev">
            <h1>Site Under Constrution</h1>
            <div class="container">
                <div class="subtitle">
                We are working on our new website. Click the button below to keep yourself busy as you wait.
            </div>
            </div>
            <button @click="openNewTab()" class="dev-btn">
                Click me!
            </button>
        </div>
    </div>
</template>

<!-- https://trex-runner.com/ -->

<style>
@import '../styles/Common.css';
@import '../styles/Dev.css';
</style>