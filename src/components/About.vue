<script setup>
    import { ref } from "vue";

    function openNewTab(url) {
        window.open(url, '_blank', 'noopener noreferrer');
    }
</script>

<template>
    <main>
        <div class="about">
            <div class="about-ct">
                <div class="ab-title">App <span class="purple">Showcase</span></div>
                <div class="ab-subtitle">Our public applications</div>
                
                <div class="about-wr">
                    <div class="b1">
                    <div class="container">
                        <div class="ab-card">
                            <div class="b-img-ct">
                                <img src="../assets/mpesa-fees-phone-mockup2.png" alt="Goose Grid" class="b-img">
                                
                                <div class="b-img-info">
                                    <div class="b-title">Mpesa Fees</div>
                                    <div class="b-subtitle">
                                        Mpesa transaction fees calculator android application.
                                    </div>
                                    <button @click="openNewTab('https://play.google.com/store/apps/details?id=com.wrenix.mpesafees&hl=en')" class="b-btn">Learn more</button>
                                </div>
                            </div>
                            
                        </div>
                    </div>
                </div>

                <div class="b1">
                    <div class="container">
                        <div class="ab-card">
                            <div class="b-img-ct">
                                <img src="../assets/pihole-mockup2.png" alt="Goose Grid" class="b-img">
                                
                                <div class="b-img-info">
                                    <div class="b-title">Pihole Manager</div>
                                    <div class="b-subtitle">
                                        Pihole DNS sink hole and ad-block manager application.
                                    </div>
                                    <button @click="openNewTab('https://play.google.com/store/apps/details?id=com.shwyfft.piholemanager&hl=en')" class="b-btn">Learn more</button>
                                </div>
                            </div>
                            
                        </div>
                    </div>
                </div>

                <div class="b1">
                    <div class="container">
                        <div class="ab-card">
                            <div class="b-img-ct">
                                <img src="../assets/goosegrid-phone-mockup2.png" alt="Goose Grid" class="b-img">
                                
                                <div class="b-img-info">
                                    <div class="b-title">Goose Grid</div>
                                    <div class="b-subtitle">
                                        KPLC electricity usage and purchase tracker.
                                    </div>
                                    <button @click="openNewTab('https://play.google.com/store/apps/details?id=com.wrenix.goosegrid&hl=en')" class="b-btn">Learn more</button>
                                </div>
                            </div>
                            
                        </div>
                    </div>
                </div>
                </div>
            </div>
        </div>
    </main>
</template>

<style>
@import '../styles/About.css';
@import '../styles/Common.css';
</style>