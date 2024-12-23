<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Bona+Nova+SC:ital,wght@0,400;0,700;1,400&family=Inter:ital,opsz,wght@0,14..32,100..900;1,14..32,100..900&family=PT+Sans:ital,wght@0,400;0,700;1,400;1,700&family=Roboto+Slab:wght@100..900&family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&family=Young+Serif&display=swap");

.boxed {
  background-image: url("../../assets/slider-activewear-1.jpg");
}

.welcome {
  padding: 300px 100px;
  width: 1540px;
  margin: 0 auto;
}

.welcome h1 {
  font-size: 80px;
  line-height: 96px;
  font-family: "Young Serif", serif;
  margin: 0;
  padding: 0;
  font-weight: 700;
  color: #000;
}
.welcome p {
  color: #333;
  font-size: 30px;
  font-weight: 500;
  margin-bottom: 30px;
}

.welcome a {
  color: #000;
  background-color: #fff;
  padding: 15px 20px;
  font-size: 18px;
  font-weight: 400;
  border-radius: 50px;
  transition: all 0.5s;
}

.welcome a:hover {
  color: #fff;
  background-color: #000;
}

.welcome a span {
  font-weight: 600;
}
</style>

<template>
  <!-- welcome -->
  <div class="boxed">
    <div class="welcome">
      <div class="welcome-content">
        <h1>
          Living
          <br />
          on a cloud.
        </h1>
        <p>You have to feel it to believe it.</p>
        <a href="#">Shop collection&nbsp;&nbsp;<span>></span> </a>
      </div>
    </div>
  </div>
</template>

<script setup></script>
