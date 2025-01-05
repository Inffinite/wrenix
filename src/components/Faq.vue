<script setup>
import { ref, onMounted } from "vue";
import { gsap } from 'gsap';
const faqs = ref(
    [
        {
            "id": 1,
            "ftitle": "What is your typical development process for a mobile app project?",
            "ffaq": "We begin by carefully listening to our clients' needs and understanding their specific challenges. Following this, we conduct thorough research and analysis to identify the most effective and efficient solutions. We then present our clients with a detailed, professional recommendation outlining our approach to address their unique requirements.",
            "active": false,
        },
        {
            "id": 2,
            "ftitle": "How do you ensure the security and privacy of my app's data?",
            "ffaq": "We ensure the security and privacy of your app's data through strong encryption, secure authentication, and regular security audits. We follow industry best practices, including data anonymization and minimization, to protect sensitive information.",
            "active": false,
        },
        {
            "id": 3,
            "ftitle": "What are your rates and pricing models for app development?",
            "ffaq": "We customize our rates based on the specific requirements of each project and the value it will deliver to our clients.",
            "active": false,
        },
    ]
);

function handleFaq(id){
    console.log("Running: " + id)
    for (let i = 0; i < faqs.value.length; i++) {
        if(faqs.value[i].id == id){
            console.log("Found")
            // await gsap.to('.fq-card-subtitle', { duration: 0.5, opacity: 1, ease: "power2.inOut", });
            faqs.value[i].active = !faqs.value[i].active
        } else {
            // await gsap.to('.fq-card-subtitle', { duration: 0.5, opacity: 0, ease: "power2.inOut", });
            faqs.value[i].active = false
        }
    }
}

function movy(){
    gsap.to('.fq-card-icon', { duration: 1, rotation: 180 });
}


</script>

<template>
    <main>
        <div class="faq">
                <div class="fq-wr">
                    <div class="fq-title"><span class="purple">Frequently</span> asked questions</div>
                    <div class="fq-subtitle">
                        Have questions? We're here to help.
                    </div>
                    <div class="fq-card-wr">
                        <div v-for="faq in faqs" :key="faq.id" @click="handleFaq(faq.id)" class="fq-card">
                            <div>
                                <svg v-if="faq.active == false" class="fq-card-icon" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor">
                                <path stroke-linecap="round" stroke-linejoin="round" d="M12 9v6m3-3H9m12 0a9 9 0 1 1-18 0 9 9 0 0 1 18 0Z" />
                                </svg>

                                <svg v-if="faq.active == true" class="fq-card-icon" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor">
                                <path stroke-linecap="round" stroke-linejoin="round" d="M15 12H9m12 0a9 9 0 1 1-18 0 9 9 0 0 1 18 0Z" />
                                </svg>
                            </div>
                            <div>
                                <div class="fq-card-head">
                                <div class="fq-head">
                                    <div class="fq-head-title">
                                        {{ faq.ftitle }}
                                    </div>
                                </div>
                            </div>
                            <div v-if="faq.active == true" class="fq-card-subtitle">
                                    {{ faq.ffaq }}
                            </div>
                            </div>
                            <!-- <div class="fq-line"></div> -->
                        </div>
                    </div>

                    <!-- <div class="fq-more">
                        <div class="fq-more-title">
                            Still have questions?
                        </div>
                        <div class="fq-more-subtitle">
                            Can't find the answer you are looking for?
                        </div>
                        <div class="container">
                            <button class="fq-more-btn">Get in touch</button>
                        </div>
                    </div> -->
                </div>
        </div>
    </main>
</template>

<style>
@import '../styles/Common.css';
@import '../styles/Faq.css';
</style>