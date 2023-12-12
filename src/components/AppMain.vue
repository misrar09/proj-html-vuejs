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
                <button class="call_to_act">Buy Avada today <i class="fa-solid fa-arrow-right"></i></button>
                <button class="play_btn"><i class="fa-solid fa-play"></i></button>
                <button class="prebuilts"><i class="fa-solid fa-mountain"><br><span>Prebuilts</span></i></button>
                <button class="buy_now"><i class="fa-solid fa-cart-shopping fa-flip-horizontal"><br><span>Buy
                            Now</span></i></button>
            </div>
        </section>
    </div>
    <section class="services">
        <div class="container">

            <div class="cards d-flex justify-content-between  ">
                <div class="card">
                    <img src="../assets/img/service6-2x.jpg" alt="service6">
                    <h4>Crossfit workout</h4>
                    <h5>Push your limits</h5>
                </div>
                <div class="card">
                    <img src="../assets/img/box1-2x.jpg" alt="service6">
                    <h4>Crossfit workout</h4>
                    <h5>Push your limits</h5>
                </div>
                <div class="card">
                    <img src="../assets/img/box3-2x.jpg" alt="service6">
                    <h4>Crossfit workout</h4>
                    <h5>Push your limits</h5>
                </div>
            </div>

            <div class="qoute1">
                <h1>"How you respond to the challenge in the second half will determine what you become after the game,
                    wheter you are a winner or a loser."</h1>
                <!-- todo: add waves -->
                <div class="qoute_author">
                    <p class="text-center">
                        <img src="../assets/img/avatar-1-2x.jpg" alt="">
                        <span><strong>Brad Johnson</strong></span>
                        <span>Las Vegas</span>
                    </p>
                </div>
            </div>
        </div>
    </section>

    <section class=" row online_advice"></section>
    <section class=" row mailing_list"></section>
    <section class=" row information"></section>
    <section class=" row articles"></section>
    <section class=" row call_to_action"></section>
    <section class=" row other_info"></section>
    <section class=" row workout_of_the_day"></section>
</template>

<style scoped lang="scss">
.jumbotron {
    height: 30rem;
    width: 100vw;
    background-image: linear-gradient(to left, transparent, transparent, #0000007a, black, black, black), url(../assets/img/slider82x-scaled.jpg);
    background-size: 96%;
    position: relative;

}

/* JUMBTRON SECTION STYLE */
.jumbo_left {
    margin: 5rem 0;

    h1 {
        padding: 1rem 0;
        font-size: 3.5rem;
    }

    h6 {
        color: red;
        font-size: 1.3rem;
    }



    p {
        padding: 1rem 0;
        color: grey;
    }
}

// importo variabili
// @use './styles/partials/variables' as *;


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

    i {
        padding-left: 0.5rem;
    }
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


/* SERVICES SECTION STYLE */
.services {
    background-image: linear-gradient(to bottom right, blue, red);
    margin-top: 1.5rem;

    div.cards {
        position: relative;
        margin-bottom: 1.5rem;
        top: -4rem;

        .card {
            width: 20rem;
            height: 22rem;
            border: none;
            background-color: transparent;

            img {
                width: 100%;
                height: 100%;
                border-radius: 5px 5px 40px 0;
            }

            &::before {
                content: '';
                position: absolute;
                top: 0;
                right: 0;
                bottom: 0;
                left: 0;
                background: linear-gradient(to bottom, transparent, rgba(0, 0, 0, 0.514));
                z-index: 1;
                border-radius: 5px 5px 40px 0;
            }

            h4 {
                color: white;
                position: absolute;
                bottom: 3rem;
                padding-left: 2rem;
                z-index: 1;
            }

            h5 {
                color: yellow;
                position: absolute;
                bottom: 1rem;
                padding-left: 2rem;
                z-index: 1;

            }

        }

    }

    .qoute1 {
        h1 {
            text-align: center;
            padding: 1rem 5rem;
            margin-bottom: 2rem;
        }

        div {
            padding-bottom: 2rem;

            img {
                width: 4rem;
                border-radius: 50rem;
            }

            span {
                padding: 0.5rem;
            }

        }
    }


}
</style>