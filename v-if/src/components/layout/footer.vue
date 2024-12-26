<style scoped>
.footer-area {
  border-top: 1px solid #ccc;
}

footer {
  height: 320px;
  padding: 50px 0px 0;
  display: flex;
  justify-content: space-between;
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
  <section class="footer-area">
    <footer class="footer boxed">
      <div class="footer-text">
        <div class="logo">
          <img
            src="https://nextash.com/assets/nextash_v2/images/logos/logo.png"
            width="50px"
            alt="Footer logo"
          />
        </div>
        <p>
          {{ footerContent }}
        </p>
      </div>
      <div class="footer-link">
          <li v-for="link in footerLinks1" :key="link">
            <a :href="link.url">{{ link.text }}</a>
          </li>
      </div>
      <div class="footer-link">
        <li v-for="link in footerLinks2" :key="link">
          <a :href="link.url">{{ link.text }}</a>
        </li>
      </div>
      <div class="footer-link">
        <li v-for="link in footerLinks3" :key="link">
          <a :href="link.url">{{ link.text }}</a>
        </li>
      </div>
    </footer>
  </section>
</template>

<script setup>
const footerContent = "Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptas id tenetur ab Iure odit magni quia incidunt tenetur aspernatur quisquam."

const footerLinks1 = [
  {
    url: "#",
    text: "Home",
  },
  {
    url: "#",
    text: "About",
  },
  {
    url: "#",
    text: "Services",
  },
  {
    url: "#",
    text: "Blog",
  },
  {
    url: "#",
    text: "Contact",
  },
];
const footerLinks2 = [
  {
    url: "#",
    text: "Home",
  },
  {
    url: "#",
    text: "About",
  },
  {
    url: "#",
    text: "Services",
  },
  {
    url: "#",
    text: "Contact",
  },
];
const footerLinks3 = [
  {
    url: "#",
    text: "Home",
  },
  {
    url: "#",
    text: "About",
  },
  {
    url: "#",
    text: "Services",
  },
  {
    url: "#",
    text: "Blog",
  },
];
</script>
