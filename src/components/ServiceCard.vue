<script setup>
const props = defineProps({
    // 1 --> Software dev
    // 2 --> UI/UX
    // 3 --> Graphic design
    iconType: String,
    title: String,
    options: Array
});
</script>

<template>
    <main>
        <div>
            <div class="container">
                <div class="s-fade"></div>
            </div>
            <div class="s-card">
                <div class="container">
                    <div class="service-icon-container">
                        <svg v-if="(props.iconType == '1')" xmlns="http://www.w3.org/2000/svg" fill="none"
                            viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="service-icon">
                            <path stroke-linecap="round" stroke-linejoin="round"
                                d="M6.75 7.5l3 2.25-3 2.25m4.5 0h3m-9 8.25h13.5A2.25 2.25 0 0021 18V6a2.25 2.25 0 00-2.25-2.25H5.25A2.25 2.25 0 003 6v12a2.25 2.25 0 002.25 2.25z" />
                        </svg>


                        <svg v-if="(props.iconType == '2')" xmlns="http://www.w3.org/2000/svg" fill="none"
                            viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="service-icon">
                            <path stroke-linecap="round" stroke-linejoin="round"
                                d="M10.5 1.5H8.25A2.25 2.25 0 006 3.75v16.5a2.25 2.25 0 002.25 2.25h7.5A2.25 2.25 0 0018 20.25V3.75a2.25 2.25 0 00-2.25-2.25H13.5m-3 0V3h3V1.5m-3 0h3m-3 18.75h3" />
                        </svg>

                        <svg v-if="(props.iconType == '3')" xmlns="http://www.w3.org/2000/svg" fill="none"
                            viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="service-icon">
                            <path stroke-linecap="round" stroke-linejoin="round"
                                d="M21 7.5l-2.25-1.313M21 7.5v2.25m0-2.25l-2.25 1.313M3 7.5l2.25-1.313M3 7.5l2.25 1.313M3 7.5v2.25m9 3l2.25-1.313M12 12.75l-2.25-1.313M12 12.75V15m0 6.75l2.25-1.313M12 21.75V19.5m0 2.25l-2.25-1.313m0-16.875L12 2.25l2.25 1.313M21 14.25v2.25l-2.25 1.313m-13.5 0L3 16.5v-2.25" />
                        </svg>
                    </div>
                </div>

                <div class="service-title">{{ props.title }}</div>

                <div class="service-options-wr">
                    <div v-for="(option, i) in props.options" :key="i" class="container">
                        <div class="service-option">
                            <!-- <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24"
                                                    stroke-width="1.5" stroke="currentColor" class="service-option-icon">
                                                    <path stroke-linecap="round" stroke-linejoin="round"
                                                        d="M9 12.75L11.25 15 15 9.75M21 12a9 9 0 11-18 0 9 9 0 0118 0z" />
                                                </svg> -->
                            {{ option }}
                        </div>
                    </div>
                </div>

                <div class="container">
                    <button class="highlight-btn">Learn more</button>
                </div>
            </div>
        </div>
    </main>
</template>

<style>
@import "../styles/Services.css";
@import "../styles/Common.css";
</style>