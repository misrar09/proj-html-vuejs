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
    <!-- JUMBOTRON SECTION -->
    <section class="jumbotron">
        <div class="container">
            <div class="row">
                <div class="col-6 jumbo_left">
                    <h6>Certified fitness professionals</h6>
                    <h1>Take control of your health</h1>
                    <img src="../assets/img/zigzag yb.png" alt="">
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit Corrupti reprehenderit ulla</p>
                    <button class="visit_yt_btn"><i class="px-2 fa-brands fa-youtube"></i> Visit my YouTube
                        channel</button>
                    <button class="call_to_act">Buy Avada today <i class="fa-solid fa-arrow-right"></i></button>
                    <button class="play_btn"><i class="fa-solid fa-play"></i></button>
                    <div class="side_btn">
                        <button class="prebuilts"><i class="fa-solid fa-mountain"><br><span>Prebuilts</span></i></button>
                        <button class="buy_now"><i class="fa-solid fa-cart-shopping"><br><span>Buy Now</span></i></button>
                    </div>
                </div>
            </div>
        </div>
    </section>
    <!-- SERVICES SECTION -->
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
                    <h4>New gym apparel</h4>
                    <h5>Look good, feel good</h5>
                </div>
                <div class="card">
                    <img src="../assets/img/box3-2x.jpg" alt="service6">
                    <h4>Team training</h4>
                    <h5>Find a partner</h5>
                </div>
            </div>
            <div class="qoute1">
                <h1>"How you respond to the challenge in the second half will determine what you become after the game,
                    wheter you are a winner or a loser."</h1>
                <!-- todo: add waves -->
                <div class="qoute_author">
                    <p class="text-center">
                        <img src="../assets/img/avatar-1-2x.jpg" alt="">
                        <span class="text-white"><strong>Brad Johnson</strong></span>
                        <span class="lasvegas">Las Vegas</span>
                    </p>
                </div>
            </div>
        </div>
    </section>
    <!-- ONLINE ADVICE SECTION -->
    <section class="online_advice">
        <div class="row">

            <div class="col-6 img_wrapper">
                <img src="../assets/img/service15-2x.jpg" alt="image">
                <button class="play_btn2"><i class="fa-solid fa-play"></i></button>
            </div>
            <div class="col-6 text-wrapper">
                <h5>Tune up your workout</h5>
                <h2>The best health & fitness advice online</h2>
                <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Dolor nesciunt blanditiis modi! Voluptates amet
                    deleniti magni</p>
                <button class="visit_yt_btn_red"><i class="px-2 fa-brands fa-youtube"></i> Visit my YouTube
                    channel</button>
            </div>
        </div>
    </section>
    <!-- PLAYLIST SECTION -->
    <section class="playlist">
        <div class="container">
            <div class="text d-flex justify-content-between mb-2 pt-5">
                <h5>Featured Playlists</h5>
                <h6>View all videos <i class="fa-solid fa-angle-right"></i></h6>
            </div>

            <div class="row vid_cards">
                <div class="col vid_card">
                    <img src="../assets/img/video2-2x.jpg" alt="">
                    <button class="play_btn_sml"><i class="fa-solid fa-play"></i></button>
                    <h6>Thighs & glute workout</h6>
                    <p>Increase your mobility</p>
                </div>
                <div class="col vid_card">
                    <img src="../assets/img/video7-2x.jpg" alt="">
                    <button class="play_btn_sml"><i class="fa-solid fa-play"></i></button>
                    <h6>Thighs & glute workout</h6>
                    <p>Increase your mobility</p>
                </div>
                <div class="col vid_card">
                    <img src="../assets/img/video9-2x.jpg" alt="">
                    <button class="play_btn_sml"><i class="fa-solid fa-play"></i></button>
                    <h6>Thighs & glute workout</h6>
                    <p>Increase your mobility</p>
                </div>
            </div>
        </div>
    </section>
    <!-- MAIL LIST SECTION -->
    <section class=" mailing_list">
        <div class="container">
            <div class="row">
                <div class="col-8 mail_today">
                    <h6>Join our mailing list today</h6>
                    <h1>Insider offers & flash sales in your inbox every week.</h1>
                    <i class="fa-solid fa-arrow-trend-up"></i>
                    <input type="text" placeholder="    Insert your email...*">
                    <button class="subscribe">Subscribe</button>
                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Adipisci voluptates eius ipsum temporibus.
                        Qui delectus, fugiat quaerat sunt molestias facilis cumque distinctio hic?</p>
                </div>
            </div>
        </div>
    </section>
    <!-- OPTIONS SECTION -->
    <section class="options">
        <div class="container">
            <div class="row option_cards gap-5">
                <div class="col option_card">
                    <i class="fa-solid fa-handshake-simple"></i>
                    <h3>Team training</h3>
                    <h4>Find a partner</h4>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quas odit ullam consequatur, non ab
                        voluptates! Minima obcaecati voluptatem?</p>
                    <h5>Find a partner <i class="fa-solid fa-angle-right"></i></h5>
                </div>
                <div class="col option_card">
                    <i class="fa-solid fa-dumbbell"></i>
                    <h3>Crossfit workout</h3>
                    <h4>Push your limits</h4>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quas odit ullam consequatur, non ab
                        voluptates! Minima obcaecati voluptatem?</p>
                    <h5>Learn about Crossfit <i class="fa-solid fa-angle-right"></i></h5>
                </div>
                <div class="col option_card">
                    <i class="fa-solid fa-person-half-dress"></i>
                    <h3>Weight loss plan</h3>
                    <h4>Shed those pounds</h4>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quas odit ullam consequatur, non ab
                        voluptates! Minima obcaecati voluptatem?</p>
                    <h5>Schedule a workout <i class="fa-solid fa-angle-right"></i></h5>
                </div>
            </div>
        </div>
    </section>
    <!-- LASTEST ARTICLES SECTION -->
    <section class="articles">
        <div class="container">
            <div class="d-flex justify-content-between mb-2 pt-5">
                <h5>Latest articles</h5>
                <h6>Read all articles <i class="fa-solid fa-angle-right"></i></h6>
            </div>
            <div class="row article_cards gap-4">
                <div class="col article_card">
                    <img src="../assets/img/blog4-2x.jpg" alt="">
                    <h6>The best protein shake</h6>
                    <p><span>By</span>admin <span>| November 26th, 2019 |</span> Gym</p>
                </div>
                <div class="col article_card">
                    <img src="../assets/img/blog1-2x.jpg" alt="">
                    <h6>Ultimate cardio workout</h6>
                    <p><span>By</span>admin <span>| November 26th, 2019 |</span> Gym</p>
                </div>
                <div class="col article_card">
                    <img src="../assets/img/blog3-2x.jpg" alt="">
                    <h6>New juices available now</h6>
                    <p><span>By</span>admin <span>| November 26th, 2019 |</span> Gym</p>
                </div>
            </div>
        </div>
    </section>
    <!-- CALL TO ACTION SECTION -->
    <section class="call_to_action">
        <div class="content">
            <h1>"I've failed over and over again in my life. And that is why I succeed."</h1>
            <!-- todo waves -->
            <p class="mt-5">Lorem ipsum dolor sit amet consectetur adipisicing elit. Vitae facilis, mollitia tenetur
                recusandae hic
                neque
                earum cum repellat perferendis quaerat? Necessitatibus dolorem porro iusto officiis.</p>
            <button class="mt-2 call_to_act">Buy Avada today <i class=" ps-2 fa-solid fa-angle-right"></i></button>
        </div>
    </section>
    <!-- SPONSORS LIST SECTION -->
    <section class="sponsors">
        <div class="container">
            <div class="row sponsor_cards pt-5">
                <div class="col-3 sponsor_card">
                    <img src="../assets/img/sponsor-1-2x.png" alt="">
                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.
                        amet
                        accusamus magnam itaque ducimus.!</p>
                    <h6>Visit Yoga Studio <i class="fa-solid fa-angle-right"></i></h6>
                </div>
                <div class="col-3 sponsor_card">
                    <img src="../assets/img/sponsor-2-2x.png" alt="">
                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.
                        amet
                        accusamus magnam itaque ducimus.!</p>
                    <h6>Visit Yoga Studio <i class="fa-solid fa-angle-right"></i></h6>
                </div>
                <div class="col-3 sponsor_card">
                    <img src="../assets/img/sponsor-3-2x.png" alt="">
                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.
                        amet
                        accusamus magnam itaque ducimus.!</p>
                    <h6>Visit Yoga Studio <i class="fa-solid fa-angle-right"></i></h6>
                </div>
                <div class="col-3 sponsor_card">
                    <img src="../assets/img/sponsor-4-2x.png" alt="">
                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.
                        amet
                        accusamus magnam itaque ducimus.!</p>
                    <h6>Visit Yoga Studio <i class="fa-solid fa-angle-right"></i></h6>
                </div>
            </div>
        </div>
    </section>
    <!-- WORKOUT OF THE DAY SECTION -->
    <section class="workout_of_the_day">
        <div class="wrapper">
            <button class="play_btn3"><i class="fa-solid fa-play"></i></button>
            <h1>Crossfit workout of the day</h1>
            <h2>November 15th, 2019</h2>
            <h6>View all videos<i class="ps-2 fa-solid fa-arrow-right"></i></h6>
        </div>
    </section>
</template>


<!-- ***************************************************************** -->

<style scoped lang="scss">
/* JUMBOTRON SECTION STYLES */
.jumbotron {
    height: 35rem;
    margin-bottom: 5rem;
    /* width: 100vw */
    background-image: linear-gradient(to left, transparent, transparent, #0000007a, black, black, black), url(../assets/img/slider82x-scaled.jpg);
    background-size: cover;
    position: relative;

}

.jumbo_left {
    margin: 5rem 0;

    h1 {
        padding: 1rem 0;
        font-size: 4rem;
        color: white;
    }

    h6 {
        color: #FF414B;
        font-size: 1.3rem;
    }

    p {
        padding: 1rem 0;
        color: grey;
        font-size: 1.5rem;
    }

    img {
        width: 5rem;
    }

    .visit_yt_btn {
        width: 18rem;
        height: 3.5rem;
        border: none;
        border-radius: 5rem;
        background-color: #4154ff;
        color: white;
        margin-right: 0.8rem;

        &:hover {
            background-color: #FF414B;
        }
    }

    .call_to_act {
        width: 12rem;
        height: 3.5rem;
        border: 1px solid gray;
        border-radius: 5rem;
        background-color: black;
        color: white;

        &:hover {
            background-color: white;
            color: black;
        }

        i {
            padding-left: 0.5rem;
        }
    }

    .play_btn {
        width: 6rem;
        height: 6rem;
        border-radius: 100%;
        color: #4154ff;
        border: none;
        position: absolute;
        right: 13rem;
        top: 11rem;

        &:hover {
            color: #FF414B;
        }
    }

    .prebuilts,
    .buy_now {
        width: 4rem;
        height: 4rem;
        border: none;
        position: fixed;
        border-radius: 0.5rem;
        right: 1rem;
        font-size: 1.2rem;
        padding: 0.5rem;
        z-index: 1;

        span {
            font-size: 0.4rem;
        }
    }

    .prebuilts {
        top: 7.5rem;
    }

    .buy_now {
        top: 12rem;
    }
}



/* SERVICES SECTION STYLE */
.services {
    background-image: linear-gradient(to bottom right, blue, #FF414B);
    margin-top: 1.5rem;
    height: 48rem;

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
                transition: transform 0.3s ease-in-out;

                &:hover {
                    transform: scale(1.2);
                }
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
                font-weight: bold;
                position: absolute;
                bottom: 3rem;
                padding-left: 2rem;
                z-index: 1;
            }

            h5 {
                font-weight: bold;
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
            color: white;
        }

        div {
            padding-bottom: 2rem;

            img {
                width: 4rem;
                border-radius: 50rem;
            }

            span {
                padding: 0.5rem;
                color: rgb(197, 197, 197);
            }
        }
    }

}



/* ONLINE ADVICE SECTION STYLES */
.online_advice {
    background-color: white;
    height: 40rem;
    position: relative;

    .img_wrapper {
        position: relative;

        img {
            width: 90%;
            position: absolute;
            top: -3rem;
            border-radius: 5px 5px 40px 0;
        }

        .play_btn2 {
            width: 5rem;
            height: 5rem;
            border-radius: 100%;
            color: #4154ff;
            background-color: white;
            border: none;
            position: absolute;
            left: 50%;
            top: 50%;
            transform: translate(-50%, -50%);

            &:hover {
                color: #FF414B;
            }
        }
    }

    .text-wrapper {
        padding: 6rem;

        h2 {
            color: black;
            font-size: 3.5rem;
            margin-bottom: 2rem;
        }

        h5 {
            color: #4154ff;
            font-size: 1.5rem;
            margin-bottom: 2rem;
        }

        p {
            color: gray;
            margin-bottom: 1.5rem;
        }

        .visit_yt_btn_red {
            width: 18rem;
            height: 3.5rem;
            border: none;
            border-radius: 5rem;
            background-color: red;
            color: white;
            margin-right: 0.8rem;

            &:hover {
                background-color: #FF414B;
            }
        }
    }
}


/* PLAYLIST SECTION STYLES */
.playlist {
    height: 40rem;
    padding-top: 5rem;
    background-color: white;

    .vid_cards {
        margin-bottom: 2rem;
    }

    .vid_card {
        /* width: 20rem; */
        text-align: center;
        line-height: 0.8rem;
        position: relative;

        img {
            width: 100%;
            border-radius: 5px 5px 40px 0;
        }

        .play_btn_sml {
            width: 3rem;
            height: 3rem;
            border-radius: 100%;
            color: #4154ff;
            background-color: white;
            border: none;
            position: absolute;
            top: 40%;
            left: 50%;
            transform: translate(-50%, -50%);

            &:hover {
                color: #FF414B;
            }
        }

        h6 {
            font-weight: bold;
            padding-top: 1rem;
        }

        p {
            color: #4154ff;
            font-size: 0.95rem;
        }
    }
}

/* MAIL LIST SECTION STYLES */
.mailing_list {
    height: 45rem;
    /* width: 100vw; */
    background-image: linear-gradient(to left, transparent, transparent, #0000007a, black, black, black), url(../assets/img/banner1-2x.jpg);
    background-size: cover;
    background-position: right;
    background-repeat: no-repeat;
    position: relative;
    margin-bottom: 4rem;
}

.mail_today {
    margin: 5rem 0;

    h1 {
        padding: 1rem 0;
        font-size: 3.5rem;
        color: white;
    }

    h6 {
        color: #FF414B;
        font-size: 1.3rem;
        margin-bottom: 1rem;
    }

    p {
        padding: 1rem 0;
        color: grey;
        font-size: 1.5rem;
    }

    .subscribe {
        width: 14rem;
        height: 3.5rem;
        border: none;
        border-radius: 5rem;
        background-color: #4154ff;
        color: white;
        margin-right: 0.8rem;

        &:hover {
            background-color: #FF414B;
        }
    }

    input {
        width: 30rem;
        height: 3.5rem;
        border-radius: 5rem;
        margin-right: 1.5rem;
        margin-top: 2rem;
        margin-bottom: 2rem;
    }
}

/* OPTONS SECTION STYLES */
.options {
    height: 40rem;

    .option_cards {
        .option_card {
            height: 35rem;
            border: 4px solid #4154ff;
            color: white;
            padding: 3rem;
            text-align: center;
            margin-bottom: 4rem;
            transition: transform 0.3s ease-in-out;

            &:hover {
                transform: scale(1.1);
            }

            i {
                font-size: 4rem;
                margin-bottom: 3rem;
                color: rgb(204, 202, 202)
            }

            h3 {
                font-size: 2rem;
            }

            h4 {
                color: yellow;
                font-size: 1.5rem;
                margin-bottom: 4rem;
            }

            h5 {
                font-size: 1.2rem;
                font-weight: bold;

                i {
                    font-size: 1rem;
                }
            }

            p {
                color: rgb(189, 189, 189);
                margin-bottom: 4rem;
            }
        }
    }
}

/* LASTEST ARTICLES SECTION STYLES */
.articles {
    background-color: white;
    color: black;
    height: 38rem;
    padding: 4rem 0;

    .article_cards {
        .article_card {
            line-height: 0.3rem;

            img {
                width: 100%;
            }

            h6 {
                margin: 1rem;
                font-weight: bold;
                font-size: 1.2rem;
            }

            p {
                padding-left: 1rem;
            }

            span {
                color: gray;
            }

        }
    }
}


/* CALL TO ACTION SECTION STYLES */
.call_to_action {
    height: 40rem;
    /* width: 100%; */
    background-image: linear-gradient(to bottom, transparent, transparent, #0000007a, black), url(../assets/img/banner2-2x.jpg);
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;

    .content {
        padding: 10rem 20rem;
        text-align: center;

        h1 {
            color: white;
            font-size: 3.2rem;
        }

        p {
            color: gray;
            font-size: 1.5rem;
            margin-bottom: 2rem;
        }

        button {
            width: 12rem;
            height: 3rem;
            background-color: #4154ff;
            color: white;
            border-radius: 5rem;
            border: none;

            &:hover {
                background-color: #FF414B;
            }
        }
    }

}

/* SPONSOR LIST SECTION STYLES */
.sponsors {
    height: 30rem;
    background-color: white;
    padding: 2rem 0;

    .sponsor_cards {
        .sponsor_card {
            padding: 2rem;
            text-align: center;

            img {
                width: 9rem;
                margin-bottom: 1.5rem;
            }

            p {
                color: grey;
                margin-bottom: 1.5rem;
            }
        }
    }
}

/* WORKOUT OF THE DAY SECTION STYLES */
.workout_of_the_day {
    height: 35rem;
    background-image: linear-gradient(to bottom right, rgba(0, 13, 128, 0.329), rgba(2, 2, 95, 0.479), rgba(255, 0, 0, 0.308)), url(../assets/img/banner14-2x.jpg);
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    position: relative;
    text-align: center;

    .wrapper {
        padding: 7rem;

        h1 {
            color: white;
            font-size: 3rem;
        }

        h2 {
            color: yellow;
            margin-bottom: 1rem;
        }

        h6 {
            color: white;
        }

        .play_btn3 {
            width: 5rem;
            height: 5rem;
            border-radius: 100%;
            color: #4154ff;
            background-color: white;
            border: none;
            margin-bottom: 1rem;

            &:hover {
                color: #FF414B;
            }

            /*             position: absolute;
            left: 50%;
            top: 50%;
            transform: translate(-50%, -50%); */
        }
    }
}
</style>