<template>
    <div>
        <div class="section pt-5">
            <div class="row justify-content-center">
                <div class="col-6">
                    <div class="section-title d-flex flex-column">

                        <div class="title">
                            <h2>Specialists In Modern Construction</h2>
                        </div>

                        <div class="div-line"></div>
                    </div>
                    <div class="title-description">
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Adipisci quibusdam magni iure
                            facilis
                            omnis blanditiis expedita, porro repellendus! Deserunt minima praesentium quas commodi.

                        </p>
                    </div>
                </div>
            </div>


            <div class="custom_padding">
                <div class="row justify-content-center mt-5">

                    <div class="col-12 col-sm-12 col-md-6 col-lg-3" v-for="card in cardList" :key="card.icon">

                        <div class="card" @pointerenter="hover = !hover">
                            <div class="mt-4">
                                <i :class="card.icon" v-if="hover"></i>
                                <button type="button" class="my-btn btn btn-light m-2 position-btn" v-else>{{ card.btn }}
                                </button>
                            </div>
                            <h2 class="title-card p-2" v-if="hover"> {{ card.title }} </h2>
                            <h5 v-else> {{ card.titleBis }}</h5>

                            <p class="card-info p-2"> {{ card.info }} </p>

                        </div>
                    </div>


                </div>


            </div>

        </div>


        <div class="br"></div>


        <div class="bg-curved">
            <div class="data">
                <div class="row justify-content-center">
                    <div class="col-12 col-sm-12 col-md-6 col-lg-3" v-for="data in dataList" :key="data.app">
                        <i :class="data.icon"></i>
                        <h3 class="number"> {{ data.number }} </h3>
                        <p class="data-info text-white text-uppercase"> {{ data.info }} </p>
                    </div>
                </div>
            </div>
        </div>

        <div class="br br-after"></div>







    </div>
</template>


<script>
export default {


    data() {
        return {
            hover: true,



            cardList: [
                {
                    icon: "fa-regular fa-building",
                    title: "Buildings",
                    titleBis: "ARTFULLY CRAFTED",
                    info: "Quis autem vel eum iure reprederit qui in ea voluptate velit esse quam nihil molestiae consequatur ",
                    btn: "GET A QUOTE",



                },
                {
                    icon: "fa-solid fa-arrows-rotate",
                    title: "Renovate",
                    titleBis: "FRESHLY NEW",
                    info: "Quis autem vel eum iure reprederit qui in ea voluptate velit esse quam nihil molestiae consequatur ",
                    btn: "GET A QUOTE",

                }, {
                    icon: "fa-solid fa-house-chimney",
                    title: "Construct",
                    titleBis: "PERFECT LINES",
                    info: "Quis autem vel eum iure reprederit qui in ea voluptate velit esse quam nihil molestiae consequatur ",
                    btn: "GET A QUOTE",


                },
                {
                    icon: "fa-solid fa-truck",
                    title: "Exclusive",
                    titleBis: "PLANNING",
                    info: "Quis autem vel eum iure reprederit qui in ea voluptate velit esse quam nihil molestiae consequatur ",
                    btn: "GET A QUOTE",


                },

            ],

            dataList: [
                {
                    icon: "fa-solid fa-wallet",
                    number: "3534",
                    info: "Planning Applications"
                },
                {
                    icon: "fa-regular fa-building",
                    number: "896",
                    info: "Completed Projects"
                },
                {
                    icon: "fa-solid fa-users",
                    number: "172",
                    info: "Trained Professionals"
                }, {
                    icon: "fa-solid fa-globe",
                    number: "19",
                    info: "International Offices"
                },

            ]
        }
    }

}


</script>


<style lang="scss" scoped>
@import "../assets/variables.scss";

.title {
    h2 {
        padding-top: 5rem;
    }
}

.div-line {
    border: 2px solid;
    color: $primary;
    margin: auto;
    width: 200px;
    margin-bottom: 2rem;
    margin-top: 2rem;
}

.custom_padding {
    padding-left: 5rem;
    padding-right: 5rem;


    .card {
        background-color: #F5F5F5;
        margin-bottom: 1rem;
        animation: alternate-reverse;

        &:hover {
            background-color: $primary;


        }
    }
 i {
        font-size: 30px;
        border: 1px solid;
        border-radius: 50%;
        padding: 1rem;
        margin: auto;
        color: #747474;
    }

    p {
        color: #747474;
    }
}

.bg-curved {

    background-image: url("/public/img/home-244125289.jpg");
    background-size: cover;
    min-height: 600px;

    .data {
        padding-top:12rem;
        padding-bottom: 2rem;
        margin: 2rem;
    }

    i {
        color: $primary;
        font-size: 100px;
    }

    h3 {
        color: $primary
    }

    .display-none {
        display: none;
    }

}

.br {
    width: 100%;
    height: 100px;
    border-radius: 15%;
    position: relative;
    top: 100px;
    background: white;
    z-index: 2;
    transform: translateX(-50%);
    left: 50%;
}

.br-after {
    top: -50px;

}
</style>