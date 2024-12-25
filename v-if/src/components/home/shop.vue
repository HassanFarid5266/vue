<style scoped>
.shop .sec-heading {
    text-align: center;
}

.shop .shop-content {
    display: flex;
    align-items: center;
    width: 100%;
    line-height: 10px;
}

.shop .shop-content .images{
    width: 50%;
    height: fit-content;
    overflow: hidden;
}

.shop .shop-content .images img{
    width: 100%;
    transition: all 1s;
}

.shop .shop-content .images img:hover{
    scale: 1.5;
    
}

</style>

<template>
    <!-- lookbook -->
    <section class="shop sec-pedding">
        <div class="sec-heading">
            <h1>Shop the look</h1>
            <p>Inspire and let yourself be inspired, from one unique fashion to another.</p>
        </div>
        <div class="shop-content">
            <div class="images" v-for="x in lookImage" :key="x">
                <img :src="x.img" alt="">
            </div>
        </div>
    </section>
</template>

<script setup>
    const lookImage = [
        {
            img: "./src/assets/lookbook-3.jpg"
        },
        {
            img: "./src/assets/lookbook-4.jpg"
        },
    ]
</script>
 