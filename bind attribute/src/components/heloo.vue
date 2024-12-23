<script setup>
    const msg = "Hello jnb kia hal hy";
    const url = "https://nextash.com"
    const objNew = {
        id : "tmkc",
        href : "https://nextash.com"
    }
</script>

<template>
    <div>
        <h1>Hello world</h1>
        <h1>{{ msg }}</h1>
        <h1 v-bind:id="msg">Vite</h1>
        <h1 :id="msg">Vite 1</h1>
        <h1><a :href="url">vite 2</a><br></h1>
        <h1><a v-bind="objNew">vite 3</a></h1>
    </div>
</template>

<style scoped>

</style>