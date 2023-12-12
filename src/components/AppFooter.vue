<script>
import { store } from "../store.js" //state management
import register from "../debug" //per debuggare il componente da console

export default {
    name: "AppFooter",
    props: {
        postsLinkList: Array,
    },
    data() {
        return {
            store
        }
    },
    methods: {
        doThings() {
            console.log("AppComponent does things");
        }
    },
    mounted() {
        register(this); //per debuggare il componente da console
        this.doThings();
    }
}
</script>

<template>
    <div class="container sec_1">
        <div class="row">
            <div class="col text-center">
                <img src="../assets/img/logo-200x34.png" alt="logo">
                <p class="pt-4">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Tenetur veniam id quaerat sit
                    fugit omnis
                    maiores rem, doloribus perspiciatis facilis</p>
                <div class="pt-4">
                    <i class="px-2 fa-brands fa-facebook-f"></i>
                    <i class="px-2 fa-brands fa-x-twitter"></i>
                    <i class="px-2 fa-brands fa-youtube"></i>
                    <i class="px-2 fa-brands fa-instagram"></i>
                    <i class="px-2 fa-brands fa-linkedin-in"></i>
                </div>
            </div>
            <div class="col text-center">
                <h6>RECENT POSTS</h6>
                <ul class="pt-4">
                    <li v-for="postLink in postsLinkList">
                        <a href="postLink.link">{{ postLink.text }}</a>
                    </li>
                </ul>


            </div>
            <div class="col text-center">
                <h6>CONTACT INFORMATION</h6>
                <p class="pt-4"> 4746 Tipple Road Michigan 48448</p>
                <h6 class="pt-2">Mobile: 1.800.000.0000</h6>
                <h6>Email: info@your-company.com</h6>
            </div>

        </div>

    </div>
    <hr>
    <div class=" sec_2 text-center">
        <p>@Copyright 2023 - 2025 | Avade theme by <strong>ThemeFusion</strong>| All rights reserved | Powered
            by
            <strong>Boolean</strong>
        </p>
    </div>
</template>

<style scoped lang="scss">
// importo variabili
// @use './styles/partials/variables' as *;


h6 {
    font-weight: bold;
}

a,
li {
    text-decoration: none;
    list-style: none;
    color: white;
    padding-bottom: 0.5rem;

}

i {
    color: red;
}

.sec_2 {
    margin: 2rem 0;
}
</style>