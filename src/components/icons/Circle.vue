<!-- This icon is from <https://github.com/Templarian/MaterialDesign>, distributed under Apache 2.0 (https://www.apache.org/licenses/LICENSE-2.0) license-->
<script setup>
const props = defineProps({
  dimensions: Number,
});

var styling = `height: ${props.dimensions}px; width: ${props.dimensions}px;`;
</script>

<template>
  <div class="circle"></div>
</template>

<style>
@media only screen {
  .circle {
    background: linear-gradient(90deg, rgba(92, 182, 164, 0.78) -22.34%, rgba(255, 181, 16, 0.78) 195.43%);
    height: 200px;
    width: 200px;
    border-radius: 999px;
    /* backdrop-filter: blur(40px); */
    -webkit-filter: blur(15px);
    filter: blur(15px);
  }
}

@media only screen and (min-width: 40.063em) and (max-width: 64em) {
  .circle {
    background: linear-gradient(90deg, rgba(92, 182, 164, 0.78) -22.34%, rgba(255, 181, 16, 0.78) 195.43%);
    height: 400px;
    width: 400px;
    border-radius: 999px;
    /* backdrop-filter: blur(40px); */
    -webkit-filter: blur(15px);
    filter: blur(15px);
  }
}

@media only screen and (min-width: 64.063em) {
  .circle {
    background: linear-gradient(90deg, rgba(92, 182, 164, 0.78) -22.34%, rgba(255, 181, 16, 0.78) 195.43%);
    height: 400px;
    width: 400px;
    border-radius: 999px;
    /* backdrop-filter: blur(40px); */
    -webkit-filter: blur(15px);
    filter: blur(15px);
  }
}
</style>