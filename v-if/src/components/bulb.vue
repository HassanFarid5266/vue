<style scoped>
#lightDiv {
  border: dashed black 1px;
  /* display: inline-block; */
  padding-bottom: 10px;
}

button.switch {
  display: block;
}

#lightDiv {
  position: relative;
  width: 150px;
  height: 150px;
}

#lightDiv > img {
  position: relative;
  width: 100%;
  height: 100%;
}

.lighton {
  position: absolute;
  top: 7%;
  left: 10%;
  width: 80%;
  height: 80%;
  border-radius: 50%;
  background-color: #fff000;
}
</style>

<template>
  <div>
    <div id="lightDiv">
      <div class="lighton" v-show="lightOn"></div>
      <img src="https://www.w3schools.com/vue/img_lightBulb.svg" />
    </div>
    <button class="switch" v-on:click="lightOn = !lightOn">Switch light</button>
  </div>
</template>

<script setup>
import { ref } from 'vue';

const lightOn = ref(false);
</script>
