<script setup>
import HelloWorld from "./components/hello.vue";
import Blub from "./components/bulb.vue";
import Header from "./components/layout/header.vue";
import Footer from "./components/layout/footer.vue";
import Welcome from "./components/home/welcome.vue";
import Cards from "./components/home/cards.vue";
</script>

<template>
  <div>
    <Header />

    <Welcome />

    <Footer />
    <!-- <Blub /> -->
    <!-- <HelloWorld /> -->
  </div>
</template>

<style scoped></style>
