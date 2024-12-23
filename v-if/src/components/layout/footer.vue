<style scoped>
footer {
  background-color: var(--color-background);
  width: 100%;
  height: 400px;
  padding: 100px 40px 0;
  display: flex;
  justify-content: space-between;
  border-top: 1px solid #ccc;
}
.footer-text,
.footer-link {
  width: 25%;
}

.footer-text p {
  padding-right: 60px;
}

.footer-link {
  padding-left: 100px;
}

.footer-link li {
  list-style: none;
  padding: 2px;
}
</style>

<template>
  <!-- footer -->
  <footer class="footer">
    <div class="footer-text">
      <div class="logo">
        <img
          src="https://nextash.com/assets/nextash_v2/images/logos/logo.png"
          width="50px"
          alt="Footer logo"
        />
      </div>
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptas id
        tenetur ab? Iure odit magni quia incidunt tenetur aspernatur quisquam.
      </p>
    </div>
    <div class="footer-link">
      <li><a href="#">Home</a></li>
      <li><a href="#">About</a></li>
      <li><a href="#">Services</a></li>
      <li><a href="#">Blog</a></li>
      <li><a href="#">Contact</a></li>
    </div>
    <div class="footer-link">
      <li><a href="#">Home</a></li>
      <li><a href="#">About</a></li>
      <li><a href="#">Services</a></li>
      <li><a href="#">Blog</a></li>
      <li><a href="#">Contact</a></li>
    </div>
    <div class="footer-link">
      <li><a href="#">Home</a></li>
      <li><a href="#">About</a></li>
      <li><a href="#">Services</a></li>
      <li><a href="#">Blog</a></li>
      <li><a href="#">Contact</a></li>
    </div>
  </footer>
</template>

<script setup></script>
