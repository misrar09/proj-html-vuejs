<script>
import { store } from "../store.js" //state management
import register from "../debug" //per debuggare il componente da console

export default {
    name: "AppMain",
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
    <div class="container">
        <section class=" row jumbotron">
            <div class="col jumbo_left">
                <h6>Certified fitness professionals</h6>
                <h1>Take control of your health</h1>
                <i class="fa-solid fa-arrow-trend-up"></i>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit Corrupti reprehenderit ulla</p>

                <button class="visit_yt_btn"><i class="px-2 fa-brands fa-youtube"></i> Visit my YouTube
                    channel</button>
                <button class="call_to_act">Buy Avada today</button>
                <button class="play_btn"><i class="fa-solid fa-play"></i></button>
                <button class="prebuilts"><i class="fa-solid fa-mountain"><br><span>Prebuilts</span></i></button>
                <button class="buy_now"><i class="fa-solid fa-cart-shopping fa-flip-horizontal"><br><span>Buy
                            Now</span></i></button>
            </div>
        </section>
        <section class=" row services"></section>
        <section class=" row online_advice"></section>
        <section class=" row mailing_list"></section>
        <section class=" row information"></section>
        <section class=" row articles"></section>
        <section class=" row call_to_action"></section>
        <section class=" row other_info"></section>
        <section class=" row workout_of_the_day"></section>

    </div>
</template>

<style scoped lang="scss">
.jumbotron {
    height: 30rem;
    width: 100vw;
    background-image: linear-gradient(to left, transparent, transparent, black, black), url(../assets/img/slider82x-scaled.jpg);
    background-size: 96%;
    position: relative;

}

.jumbo_left {
    margin: 5rem 0;
}

// importo variabili
// @use './styles/partials/variables' as *;
h6 {
    color: red;
    font-size: 1.3rem;
}

h1 {
    padding: 1rem 0;
    font-size: 3.5rem;
}

p {
    padding: 1rem 0;
    color: grey;
}

.fa-arrow-trend-up {
    font-size: 2rem;
    color: yellow;
}

.visit_yt_btn {
    width: 18rem;
    height: 3rem;
    border: none;
    border-radius: 5rem;
    background-color: #4154ff;
    color: white;
    margin-right: 0.8rem;
}

.call_to_act {
    width: 12rem;
    height: 3rem;
    border: 1px solid gray;
    border-radius: 5rem;
    background-color: black;
    color: white;
}

.play_btn {
    width: 5rem;
    height: 5rem;
    border-radius: 100%;
    color: #4154ff;
    border: none;
    position: absolute;
    right: 13rem;
    top: 11rem;
}

.prebuilts,
.buy_now {
    width: 3.5rem;
    height: 3.5rem;
    border: none;
    position: absolute;
    border-radius: 0.5rem;
    right: 3.8rem;
    font-size: 1.2rem;
    padding: 0.5rem;

    span {
        font-size: 0.4rem;
    }
}

.prebuilts {
    top: 4rem;
}

.buy_now {

    top: 8rem;
}
</style>