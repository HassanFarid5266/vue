<style scoped>

</style>

<template>
  <div>
    <div>
      <h1 v-if="stock > 8">In Stock</h1>
      <h1 v-else-if="stock > 0">Very few left</h1>
      <h1 v-else>Out of stock</h1>
    </div>

    <br />

    <div>
      <h1 v-show="showDiv">{{ msg }}</h1>
      <h1 v-if="!showDiv">{{ error }}</h1>
    </div>

    <br />

    <div class="logos">
      <ul>
        <li>
          <figure v-for="x in logos">
            <img :src="x.url" alt="" />
            <figcaption>{{ x.name }}</figcaption>
          </figure>
        </li>
      </ul>
    </div>

    <br />
    <br />

    <div class="count">
      <button class="btn btn-primary" @click="count++">
        Count: {{ count }}
      </button>
    </div>

   
  </div>
</template>

<script setup>
import { ref } from "vue";

const stock = 10;
const showDiv = false;
const msg = "Show",
  error = "Error, Something happening here hurry up and solve it ";

const logos = [
  { url: "https://www.w3schools.com/vue/img_burrito.svg", name: "Burrito" },
  { url: "https://www.w3schools.com/vue/img_salad.svg", name: "Salad" },
  { url: "https://www.w3schools.com/vue/img_soup.svg", name: "Soup" },
  { url: "https://www.w3schools.com/vue/img_pizza.svg", name: "Pizza" },
];

const count = ref(0);

</script>
