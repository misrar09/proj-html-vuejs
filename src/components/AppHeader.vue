<script>
import { store } from "../store.js" //state management
import register from "../debug" //per debuggare il componente da console

export default {
    name: "AppHeader",
    props: {

        navBarLinks: Array,
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
    <div class=" container">
        <div class=" header row align-items-center">
            <div class="col-4">
                <img src="../assets/img/logo-200x34.png" alt="">
            </div>
            <div class="col navbar d-flex ">
                <a v-for="navLink in navBarLinks" :href="navLink.link">{{ navLink.text }}</a>
                <button class="store_new_btn" type="button">New</button>
                <button class="Schedule_btn" type="button">Schedule a workout</button>
                <i class="fa-solid fa-cart-shopping"></i>
                <i class="fa-solid fa-magnifying-glass"></i>
            </div>
        </div>
    </div>
</template>

<style scoped lang="scss">
// importo variabili
// @use './styles/partials/variables' as *;

.header {
    height: 5rem;
    width: 100%;
    gap: 5rem;

}


.navbar {

    i {
        color: gray;

        &:hover {
            color: white;
        }

    }

    a {
        text-decoration: none;
        color: grey;

        &:hover {
            color: white;
        }
    }
}

.store_new_btn {
    background-color: yellow;
    height: 1.5rem;
    width: 2rem;
    font-size: 0.7rem;
    padding: 0.2rem;
    margin-left: -1.2rem;

}

.Schedule_btn {
    border-radius: 1rem;
    border: none;
    font-size: 0.75rem;
    height: 2.5rem;
    width: 10rem;
    background-color: #4154ff;
    color: white;

    &:hover {
        background-color: #FF414B;
    }
}
</style>