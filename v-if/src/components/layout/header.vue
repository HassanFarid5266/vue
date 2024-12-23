<style lang="scss" scoped>
    header {
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 20px 40px;
        // background-color: #;
        .logo {
            img {
                filter: drop-shadow(rgba(235, 0, 0, 0.24) 10px 10px 18px);
                // box-shadow: ;
            }
        }
        nav {
            ul {
                display: flex;
                align-items: center;
                column-gap: 30px;
                li {
                    list-style-type: none;
                }
            }
        }
    }
</style>

<template>
    <!-- header -->
    <header>
        <div class="logo">
            <img :src="Company_url" width="50px " alt="Company Logo">
        </div>
        <nav class="menu">
            <ul >
                <li v-for="x in menu"><a href="#">{{ x }}</a></li>
            </ul>
        </nav>
        <div class="button">
            <button class="btn btn-primary" v-for="x in header_button" >{{ x }}</button>
        </div>
    </header>
</template>

<script setup>
    const Company_url = "https://nextash.com/assets/nextash_v2/images/logos/logo.png";

    const menu = [ 
        "Home",
        "About",
        "Services",
        "Blog",
        "Contact us",
    ]

    const header_button = [
        "Login",
        "Sign up"
    ]
</script>