<script setup>
import ReviewCard from "./ReviewCard.vue";
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

            <div class="footer">
                <div class="socials">
                    <div class="s-icon-wr">
                        <svg class="s-icon" xmlns="http://www.w3.org/2000/svg" xml:space="preserve"
                            style="enable-background:new 0 0 308 308" viewBox="0 0 308 308">
                            <path
                                d="M227.904 176.981c-.6-.288-23.054-11.345-27.044-12.781-1.629-.585-3.374-1.156-5.23-1.156-3.032 0-5.579 1.511-7.563 4.479-2.243 3.334-9.033 11.271-11.131 13.642-.274.313-.648.687-.872.687-.201 0-3.676-1.431-4.728-1.888-24.087-10.463-42.37-35.624-44.877-39.867-.358-.61-.373-.887-.376-.887.088-.323.898-1.135 1.316-1.554 1.223-1.21 2.548-2.805 3.83-4.348a140.77 140.77 0 0 1 1.812-2.153c1.86-2.164 2.688-3.844 3.648-5.79l.503-1.011c2.344-4.657.342-8.587-.305-9.856-.531-1.062-10.012-23.944-11.02-26.348-2.424-5.801-5.627-8.502-10.078-8.502-.413 0 0 0-1.732.073-2.109.089-13.594 1.601-18.672 4.802C90 87.918 80.89 98.74 80.89 117.772c0 17.129 10.87 33.302 15.537 39.453.116.155.329.47.638.922 17.873 26.102 40.154 45.446 62.741 54.469 21.745 8.686 32.042 9.69 37.896 9.69h.001c2.46 0 4.429-.193 6.166-.364l1.102-.105c7.512-.666 24.02-9.22 27.775-19.655 2.958-8.219 3.738-17.199 1.77-20.458-1.348-2.216-3.671-3.331-6.612-4.743z" />
                            <path
                                d="M156.734 0C73.318 0 5.454 67.354 5.454 150.143c0 26.777 7.166 52.988 20.741 75.928L.212 302.716a3.998 3.998 0 0 0 4.999 5.096l79.92-25.396c21.87 11.685 46.588 17.853 71.604 17.853C240.143 300.27 308 232.923 308 150.143 308 67.354 240.143 0 156.734 0zm0 268.994c-23.539 0-46.338-6.797-65.936-19.657a3.996 3.996 0 0 0-3.406-.467l-40.035 12.726 12.924-38.129a4.002 4.002 0 0 0-.561-3.647c-14.924-20.392-22.813-44.485-22.813-69.677 0-65.543 53.754-118.867 119.826-118.867 66.064 0 119.812 53.324 119.812 118.867.001 65.535-53.746 118.851-119.811 118.851z" />
                        </svg>

                        <svg class="s-icon" xmlns="http://www.w3.org/2000/svg" xml:space="preserve"
                            style="enable-background:new 0 0 53.942 53.942" viewBox="0 0 53.942 53.942">
                            <path
                                d="M53.364 40.908c-2.008-3.796-8.981-7.912-9.288-8.092-.896-.51-1.831-.78-2.706-.78-1.301 0-2.366.596-3.011 1.68-1.02 1.22-2.285 2.646-2.592 2.867-2.376 1.612-4.236 1.429-6.294-.629L17.987 24.467c-2.045-2.045-2.233-3.928-.632-6.291.224-.309 1.65-1.575 2.87-2.596.778-.463 1.312-1.151 1.546-1.995.311-1.123.082-2.444-.652-3.731-.173-.296-4.291-7.27-8.085-9.277a4.947 4.947 0 0 0-2.306-.573 4.908 4.908 0 0 0-3.49 1.445L4.7 3.986C.686 7.999-.767 12.548.379 17.506c.956 4.132 3.742 8.529 8.282 13.068l14.705 14.705c5.746 5.746 11.224 8.66 16.282 8.66h.001c3.72 0 7.188-1.581 10.305-4.698l2.537-2.537a4.908 4.908 0 0 0 .873-5.796z" />
                        </svg>

                        <svg class="s-icon" xmlns="http://www.w3.org/2000/svg" xml:space="preserve"
                            style="enable-background:new 0 0 551.034 551.034" viewBox="0 0 551.034 551.034">
                            <linearGradient id="a" x1="275.517" x2="275.517" y1="4.571" y2="549.72"
                                gradientTransform="matrix(1 0 0 -1 0 554)" gradientUnits="userSpaceOnUse">
                                <stop offset="0" style="stop-color:#e09b3d" />
                                <stop offset=".3" style="stop-color:#c74c4d" />
                                <stop offset=".6" style="stop-color:#c21975" />
                                <stop offset="1" style="stop-color:#7024c4" />
                            </linearGradient>
                            <path
                                d="M386.878 0H164.156C73.64 0 0 73.64 0 164.156v222.722c0 90.516 73.64 164.156 164.156 164.156h222.722c90.516 0 164.156-73.64 164.156-164.156V164.156C551.033 73.64 477.393 0 386.878 0zM495.6 386.878c0 60.045-48.677 108.722-108.722 108.722H164.156c-60.045 0-108.722-48.677-108.722-108.722V164.156c0-60.046 48.677-108.722 108.722-108.722h222.722c60.045 0 108.722 48.676 108.722 108.722v222.722z" />
                            <linearGradient id="b" x1="275.517" x2="275.517" y1="4.571" y2="549.72"
                                gradientTransform="matrix(1 0 0 -1 0 554)" gradientUnits="userSpaceOnUse">
                                <stop offset="0" style="stop-color:#e09b3d" />
                                <stop offset=".3" style="stop-color:#c74c4d" />
                                <stop offset=".6" style="stop-color:#c21975" />
                                <stop offset="1" style="stop-color:#7024c4" />
                            </linearGradient>
                            <path
                                d="M275.517 133C196.933 133 133 196.933 133 275.516s63.933 142.517 142.517 142.517S418.034 354.1 418.034 275.516 354.101 133 275.517 133zm0 229.6c-48.095 0-87.083-38.988-87.083-87.083s38.989-87.083 87.083-87.083c48.095 0 87.083 38.988 87.083 87.083 0 48.094-38.989 87.083-87.083 87.083z" />
                            <linearGradient id="c" x1="418.306" x2="418.306" y1="4.571" y2="549.72"
                                gradientTransform="matrix(1 0 0 -1 0 554)" gradientUnits="userSpaceOnUse">
                                <stop offset="0" />
                                <stop offset=".3" />
                                <stop offset=".6" />
                                <stop offset="1" />
                            </linearGradient>
                            <circle cx="418.306" cy="134.072" r="34.149" />
                        </svg>
                    </div>
                </div>
                <div class="container">
                    All Rights Reserved © wrenix 2022
                </div>
            </div>
        </div>
    </main>
</template>

<style>
@import "../styles/Reviews.css";
@import "../styles/Common.css";
</style>