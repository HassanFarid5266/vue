<style scoped>
.product .sec-heading {
  text-align: center;
}

.products-cards {
  display: grid;
  grid-template-columns: auto auto auto auto;
  gap: 20px;
}

.product-card {
  position: relative;
  width: 100%;
  border-radius: 25px;
  padding: 20px 30px 30px 30px;
  background: #fff;
  box-shadow: 0 0px 1px rgba(0, 0, 0, 0.1);
  border: 1px solid #cccccc34;
  z-index: 3;
  overflow: hidden;
}

.product-card .logo-cart {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.product-card .logo-cart img {
  height: 60px;
  width: 60px;
  object-fit: cover;
}

.product-card .logo-cart i {
  font-size: 27px;
  color: #707070;
  cursor: pointer;
  transition: color 0.3s ease;
}

.product-card .logo-cart i:hover {
  color: #333;
}

.product-card .main-images {
  width: 100%;
  position: relative;
}

.product-card .main-images img {
  width: 100%;
  object-fit: cover;
  height: 220px;
}

.product-card .shoe-details .shoe_name {
  font-size: 24px;
  font-weight: 500;
  color: #161616;
}

.product-card .shoe-details p {
  font-size: 12px;
  font-weight: 400;
  color: #333;
  text-align: justify;
}

.product-card .shoe-details .stars i {
  margin: 0 -1px;
  color: #333;
}

.product-card .color-price .color-option {
  display: flex;
  align-items: center;
}

.color-price {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-top: 10px;
}

.color-price .color-option .color {
  font-size: 18px;
  font-weight: 500;
  color: #333;
  margin-right: 8px;
}

.color-option .circles {
  display: flex;
}

.color-option .circles .circle {
  height: 18px;
  width: 18px;
  background: #0071c7;
  border-radius: 50%;
  margin: 0 4px;
  cursor: pointer;
  transition: all 0.4s ease;
}

.color-option .circles .circle.blue.active {
  box-shadow: 0 0 0 2px #fff, 0 0 0 4px #0071c7;
}

.color-option .circles .circle.pink {
  background: #fa1795;
}

.color-option .circles .circle.pink.active {
  box-shadow: 0 0 0 2px #fff, 0 0 0 4px #fa1795;
}

.color-option .circles .circle.yellow {
  background: #f5da00;
}

.color-option .circles .circle.yellow.active {
  box-shadow: 0 0 0 2px #fff, 0 0 0 4px #f5da00;
}

.color-price .price {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.color-price .price .price_num {
  font-size: 25px;
  font-weight: 600;
  color: #707070;
}

.color-price .price .price_letter {
  font-size: 10px;
  font-weight: 600;
  margin-top: -4px;
  color: #707070;
}

.product-card .button {
  position: relative;
  height: 50px;
  width: 100%;
  border-radius: 25px;
  margin-top: 30px;
  overflow: hidden;
}

.product-card .button .button-layer {
  position: absolute;
  height: 100%;
  width: 300%;
  left: -100%;
  /* background-image: linear-gradient(135deg, #9708cc, #43cbff, #9708cc, #43cbff); */
  background-color: transparent;
  transition: all 0.5s ease;
  border-radius: 25px;
}

.product-card .button:hover .button-layer {
  left: 0;
  background-color: #000;
}

.product-card .button button {
  position: relative;
  height: 100%;
  width: 100%;
  background: none;
  outline: none;
  border: 1px solid #ccc;
  border-radius: inherit;
  font-size: 18px;
  font-weight: 600;
  letter-spacing: 1px;
  color: #000;
  cursor: pointer;
  /* transition: all 0.5s; */
}

.product-card .button button:hover {
  color: #fff;
}

@media (max-width: 1280px) {
  .products-cards {
    grid-template-columns: auto auto;
  }

  .product-card .main-images img {
    left: 110px;
  }
}

@media (max-width: 1024px) {
  .product-card .main-images img {
    left: 12px;
  }
}

@media (max-width: 576px) {
  .products-cards {
    grid-template-columns: auto;
  }
}
</style>

<template>
  <section class="product boxed sec-pedding-bottom">
    <div class="sec-heading">
      <h1>Best Seller</h1>
      <p>
        Shop the Latest Styles: Stay ahead of the curve with our newest arrivals
      </p>
    </div>
    <div class="products-cards">
      <div class="product-card" v-for="x in image" :key="x.color">
        <div class="logo-cart">
          <img :src="logo" alt="logo" />
          <i :class="x.icon"></i>
        </div>
        <div class="main-images">
          <img
            :id="x.color"
            :class="x.color"
            :src="x.url"
            :alt="x.color"
            loading="lazy"
          />
        </div>
        <div class="shoe-details">
          <span class="shoe_name">ADDIDAS GAZE ZX</span>
          <p>
            Lorem ipsum dolor sit lorenm i amet, consectetur adipisicing elit.
            Eum, ea, ducimus!
          </p>
          <div class="stars">
            <i class="bx bxs-star"></i>
            <i class="bx bxs-star"></i>
            <i class="bx bxs-star"></i>
            <i class="bx bxs-star"></i>
            <i class="bx bx-star"></i>
          </div>
        </div>
        <div class="color-price">
          <div class="color-option">
            <span class="color">Colour:</span>
            <div class="circles">
              <span class="circle blue active" id="blue"></span>
              <span class="circle pink" id="pink"></span>
              <span class="circle yellow" id="yellow"></span>
            </div>
          </div>
          <div class="price">
            <span class="price_num">$09.00</span>
            <span class="price_letter">Nine dollar only</span>
          </div>
        </div>
        <div class="button">
          <div class="button-layer"></div>
          <button>Add To Cart</button>
        </div>
      </div>
    </div>
    <div class="b-button">
      <a href="#" class="btn btn-primary btn-pill">Load more</a>
    </div>
  </section>
</template>

<script setup>
const logo = "./src/assets/logo.jpg";

const image = [
  {
    url: "./src/assets/blue.png",
    icon: "bx bx-shopping-bag",
  },
  {
    url: "./src/assets/pink.png",
    icon: "bx bxs-store",
  },
  {
    url: "./src/assets/yellow.png",
    icon: "bx bxs-shopping-bags",
  },
];
</script>
