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

                    <div class="col-3" v-for="card in cardList" :key="card.icon">

                        <div class="card">
                            <i :class="card.icon"></i>
                            <div class="title-card"> {{ card.title }} </div>
                            <p class="card-info p-3"> {{ card.info }} </p>
                        </div>
                    </div>
                </div>
            </div>

            <div class="br"></div>


            <div class="bg-curved">
                <div class="data d-flex justify-content-center">
                    <div class="m-5" v-for="data in dataList" :key="data.app">
                        <i :class="data.icon"></i>
                        <h3 class="number"> {{ data.number }} </h3>
                        <p class="data-info text-white text-uppercase"> {{ data.info }} </p>
                    </div>
                </div>
            </div>

            <div class="br br-after"></div>

        </div>
    </div>





</template>


<script>
export default {


    data() {
        return {
            cardList: [
                {
                    icon: "fa-regular fa-building",
                    title: "Buildings",
                    info: "Quis autem vel eum iure reprederit qui in ea voluptate velit esse quam nihil molestiae consequatur "


                },
                {
                    icon: "fa-solid fa-arrows-rotate",
                    title: "Renovate",
                    info: "Quis autem vel eum iure reprederit qui in ea voluptate velit esse quam nihil molestiae consequatur "


                }, {
                    icon: "fa-solid fa-house-chimney",
                    title: "Construct",
                    info: "Quis autem vel eum iure reprederit qui in ea voluptate velit esse quam nihil molestiae consequatur "


                },
                {
                    icon: "fa-solid fa-truck",
                    title: "Exclusive",
                    info: "Quis autem vel eum iure reprederit qui in ea voluptate velit esse quam nihil molestiae consequatur "


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
    padding-left: 12rem;
    padding-right: 12rem;

    .card {
        background-color: #F5F5F5;
    }

    i {
        font-size: 30px;
        border: 1px solid;
        border-radius: 50%;
        padding: 1rem;
        margin: auto;
    }
}




.bg-curved {

    background-image: url("/public/img/home-244125289.jpg");
    background-size: cover;
    min-height: 700px;

    .data {
        padding-top: 10rem;
        margin: 2rem;
    }

    i{
        color:$primary;
        font-size:70px ;
    }
    h3 {
        color: $primary
    }

}

.br {
   width: 100%;
    height: 150px;
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





.data {
    padding-top: 8rem;
}
</style>