<script setup>
import Circle from '../components/icons/Circle.vue';

function openLink() {
    window.open("https://wa.link/mapl4a");
}
</script>

<template>
    <main>
        <div class="landing">
            <div class="container">
                <div>
                    <!-- <div class="container">
                        <canvas id="canvas" width="1000" height="300"></canvas>
                      </div> -->
                    <div class="circ1">
                        <Circle />
                        <div class="container">
                            <img src="../assets/squigly-line.png" alt="" class="w-image">
                        </div>
                        <Circle />
                    </div>

                    <div class="w-title">WELCOME TO</div>
                    <div class="container">
                        <img class="w-name" src="../assets/wrenix.svg" alt="">
                    </div>
                    <div class="w-subtitle">CREATIVE DESIGN AGENCY</div>
                </div>
            </div>

            <div class="container">
                <div class="l-desc">
                    We are a team of professional <span>Designers</span> and <span>Developers</span> in the industry.
                </div>
            </div>

            <div class="container">
                <button @click="openLink()" style="margin-top: 40px;" class="hire-btn">Lets talk</button>
            </div>

            <div style="position: relative;" class="container">
                <div class="circle2"></div>
                <div class="circle3"></div>
                <div class="options">
                    <div class="container">
                        <div class="op-item">
                            <svg class="op-icon" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                                <path
                                    d="M15.2156 5.99994L14.0943 7.12126C13.7038 7.51178 13.7038 8.14495 14.0943 8.53547C14.4848 8.92599 15.118 8.92599 15.5085 8.53547L18.337 5.70704C18.5245 5.51951 18.6299 5.26515 18.6299 4.99994C18.6299 4.73472 18.5245 4.48037 18.337 4.29283L15.5085 1.4644C15.4597 1.41559 15.4071 1.37287 15.3517 1.33626C14.9635 1.07998 14.436 1.12269 14.0943 1.4644C13.7038 1.85493 13.7038 2.48809 14.0943 2.87862L15.2156 3.99994H10.0088C5.59051 3.99994 2.00879 7.58166 2.00879 11.9999C2.00879 13.3979 2.36734 14.712 2.9975 15.8555C3.29674 16.3985 4.02656 16.4466 4.46495 16.0082C4.81428 15.6589 4.85507 15.1135 4.63482 14.6713C4.23414 13.8668 4.00879 12.9597 4.00879 11.9999C4.00879 8.68623 6.69508 5.99994 10.0088 5.99994H15.2156Z" />
                                <path
                                    d="M9.92326 21.1213L8.80194 19.9999H14.0088C18.4271 19.9999 22.0088 16.4182 22.0088 11.9999C22.0088 10.602 21.6502 9.28783 21.0201 8.14434C20.9827 8.07647 20.9385 8.01633 20.8891 7.9639C20.5429 7.59692 19.9362 7.60804 19.5526 7.99163C19.2033 8.34096 19.1625 8.88633 19.3828 9.32855C19.4328 9.42911 19.4802 9.53127 19.5247 9.63494C19.8363 10.3606 20.0088 11.1601 20.0088 11.9999C20.0088 15.3136 17.3225 17.9999 14.0088 17.9999H8.80194L9.92326 16.8786C10.3138 16.4881 10.3138 15.8549 9.92326 15.4644C9.53273 15.0739 8.89957 15.0739 8.50904 15.4644L5.68062 18.2928C5.49308 18.4804 5.38772 18.7347 5.38772 18.9999C5.38772 19.2652 5.49308 19.5195 5.68062 19.707L8.50904 22.5355C8.89957 22.926 9.53273 22.926 9.92326 22.5355C10.3138 22.1449 10.3138 21.5118 9.92326 21.1213Z" />
                            </svg>
                            <div class="op-title">Infinite</div>
                            <div class="op-subtitle">Work revisions</div>
                        </div>
                    </div>

                    <div class="op-divider"></div>

                    <div class="container">
                        <div class="op-item">
                            <svg class="op-icon" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                                <g clip-path="url(#clip0_27_265)">
                                    <path fill-rule="evenodd" clip-rule="evenodd"
                                        d="M7 10.5C9.07107 10.5 10.75 8.82107 10.75 6.75C10.75 4.67893 9.07107 3 7 3C4.92893 3 3.25 4.67893 3.25 6.75C3.25 8.82107 4.92893 10.5 7 10.5ZM7 8.5C7.9665 8.5 8.75 7.7165 8.75 6.75C8.75 5.7835 7.9665 5 7 5C6.0335 5 5.25 5.7835 5.25 6.75C5.25 7.7165 6.0335 8.5 7 8.5Z" />
                                    <path fill-rule="evenodd" clip-rule="evenodd"
                                        d="M20.75 6.75C20.75 8.82107 19.0711 10.5 17 10.5C14.9289 10.5 13.25 8.82107 13.25 6.75C13.25 4.67893 14.9289 3 17 3C19.0711 3 20.75 4.67893 20.75 6.75ZM18.75 6.75C18.75 7.7165 17.9665 8.5 17 8.5C16.0335 8.5 15.25 7.7165 15.25 6.75C15.25 5.7835 16.0335 5 17 5C17.9665 5 18.75 5.7835 18.75 6.75Z" />
                                    <path fill-rule="evenodd" clip-rule="evenodd"
                                        d="M15.4587 14.1763C15.9532 14.061 16.4691 14 17 14C18.9818 14 20.7624 14.8517 22 16.2153V18H16C16 18.7286 15.8052 19.4117 15.4649 20H22C23.1046 20 24 19.1046 24 18V16.1668C24 15.7334 23.8649 15.3068 23.5791 14.9811C21.9754 13.1536 19.6224 12 17 12C15.9266 12 14.8983 12.1933 13.948 12.547C14.3532 12.8904 14.7324 13.2632 15.0823 13.6619C15.2263 13.826 15.3513 13.9984 15.4587 14.1763ZM21.9998 16.1618C21.9998 16.1618 21.9998 16.1621 21.9999 16.1624L21.9998 16.162L21.9998 16.1618Z" />
                                    <path fill-rule="evenodd" clip-rule="evenodd"
                                        d="M12 20C13.1046 20 14 19.1046 14 18V16.1668C14 15.7334 13.8649 15.3068 13.5791 14.9811C13.1123 14.4492 12.582 13.9743 12 13.5684C10.5827 12.5798 8.85906 12 7 12C4.37758 12 2.02461 13.1536 0.420908 14.9811C0.135096 15.3068 0 15.7334 0 16.1668V18C0 19.1046 0.895431 20 2 20H12ZM7 14C8.98184 14 10.7624 14.8517 12 16.2153V18H2V16.2153C3.23758 14.8517 5.01817 14 7 14ZM11.9999 16.1624C11.9998 16.162 11.9998 16.1617 11.9998 16.1617C11.9998 16.1617 11.9998 16.1619 11.9999 16.1624ZM2.0002 16.1617C2.0002 16.1617 2.00017 16.1619 2.00014 16.1624L2.0002 16.1617ZM2.0002 16.1618C2.00019 16.1619 2.00017 16.1621 2.00014 16.1624L2.0002 16.1618Z" />
                                </g>
                                <defs>
                                    <clipPath id="clip0_27_265">
                                        <rect width="24" height="24" fill="white" />
                                    </clipPath>
                                </defs>
                            </svg>

                            <div class="op-title">Professional</div>
                            <div class="op-subtitle">Designers and developers</div>
                        </div>
                    </div>

                    <div class="op-divider"></div>

                    <div class="container">
                        <div class="op-item">
                            <svg class="op-icon" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                                <path
                                    d="M12 7.5C11.4477 7.5 11 7.94772 11 8.5V12C11 12.3573 11.1906 12.6874 11.5 12.866L14.9641 14.866C15.0239 14.9005 15.0858 14.9282 15.1488 14.9492C15.5901 15.0963 16.0885 14.9185 16.3301 14.5C16.6063 14.0217 16.4424 13.4101 15.9641 13.134L13 11.4227V8.5C13 7.94772 12.5523 7.5 12 7.5Z" />
                                <path fill-rule="evenodd" clip-rule="evenodd"
                                    d="M12 22C17.5228 22 22 17.5228 22 12C22 6.47715 17.5228 2 12 2C6.47715 2 2 6.47715 2 12C2 17.5228 6.47715 22 12 22ZM12 20C16.4183 20 20 16.4183 20 12C20 7.58172 16.4183 4 12 4C7.58172 4 4 7.58172 4 12C4 16.4183 7.58172 20 12 20Z" />
                            </svg>

                            <div class="op-title">Fast</div>
                            <div class="op-subtitle">Turnaround time</div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </main>
</template>

<style>
@import '../styles/Common.css';
@import '../styles/Landing.css';
</style>