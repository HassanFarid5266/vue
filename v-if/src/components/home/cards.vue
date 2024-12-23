<style scoped>
.collection {
  padding: 120px 0;
}

.collection .sec-heading {
  margin-block: 20px;
}

/* .collection .sec-heading h1 {
  color: var(--color-background);
  font-size: 50px;
} */

.collection-cards {
  display: grid;
  grid-template-columns: auto auto auto auto;
  gap: 20px;
}

.collection-cards .card {
  position: relative;
}

.collection-cards .card .image{
  overflow: hidden;
} 

.collection-cards .card img {
  width: 100%;
  height: 500px;
  border-radius: 8px;
  transition: all 0.8s ease-in-out;
}

.collection-cards .card img:hover {
  scale: 1.2;
}
  
.collection-cards .card .collection-content a {
  position: absolute;
  bottom: 30px;
  left: 16px;
  scale: 0.9;
  font-weight: 600;
  transition: all 0.5s ease-in-out;

}

.collection-cards .card .collection-content a:hover {
  color: #000;
  scale: 1.2;
}

.collection-cards .card .collection-content .card-badge {
  background-color: #fff;
  /* color: #fff; */
  padding: 10px 20px;
}
</style>

<template>

  
  <section class="boxed collection">
    <div class="sec-heading">
      <h1>Shop</h1>
      <p>Shop by Categories</p>
    </div>
    <div class="collection-cards">
      <article class="card" v-for="collectionCard in collectionCards" :key="collectionCard">
        <div class="image">
          <a href="#">
            <img :src="collectionCard.url" alt="" />
          </a>
        </div>

        <span class="collection-content">
          <a href="#">
            <span class="card-badge">{{ collectionCard.cardBadge }}</span>
          </a>
        </span>
      </article>
    </div>
  </section>
</template>

<script setup>
const collectionCards = [
  {
    url: "https://images.pexels.com/photos/29783666/pexels-photo-29783666/free-photo-of-elegant-woman-posing-with-fan-outdoors.jpeg?auto=compress&cs=tinysrgb&w=600&lazy=load",
    cardBadge: "Clothing",
  },
  {
    url: "https://themesflat.co/html/modave-intro/assets/images/video/cls-tiktok4.jpg",
    cardBadge: "Sunglasses",
  },
  {
    url: "https://themesflat.co/html/modave-intro/assets/images/video/cls-tiktok2.jpg",
    cardBadge: "Beauty",
  },
  {
    url: "https://themesflat.co/html/modave-intro/assets/images/video/cls-tiktok1.jpg",
    cardBadge: "Fashion",
  },
  {
    url: "https://themesflat.co/html/modave-intro/assets/images/video/cls-tiktok1.jpg",
    cardBadge: "Fashion",
  },
  {
    url: "https://themesflat.co/html/modave-intro/assets/images/video/cls-tiktok2.jpg",
    cardBadge: "Beauty",
  },
  {
    url: "https://themesflat.co/html/modave-intro/assets/images/video/cls-tiktok4.jpg",
    cardBadge: "Sunglasses",
  },
  {
    url: "https://images.pexels.com/photos/29783666/pexels-photo-29783666/free-photo-of-elegant-woman-posing-with-fan-outdoors.jpeg?auto=compress&cs=tinysrgb&w=600&lazy=load",
    cardBadge: "Clothing",
  },
  {
    url: "https://images.pexels.com/photos/29783666/pexels-photo-29783666/free-photo-of-elegant-woman-posing-with-fan-outdoors.jpeg?auto=compress&cs=tinysrgb&w=600&lazy=load",
    cardBadge: "Clothing",
  },
  {
    url: "https://themesflat.co/html/modave-intro/assets/images/video/cls-tiktok4.jpg",
    cardBadge: "Sunglasses",
  },
  {
    url: "https://themesflat.co/html/modave-intro/assets/images/video/cls-tiktok2.jpg",
    cardBadge: "Beauty",
  },
  {
    url: "https://themesflat.co/html/modave-intro/assets/images/video/cls-tiktok1.jpg",
    cardBadge: "Fashion",
  },
];
</script>
