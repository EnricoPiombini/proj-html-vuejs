<template>
    <div>
        <div class="section pt-5">
            <div class="section section-text text-center">
                <div class="section-title">
                    <h4>Specialists In Modern Construction</h4>
                </div>

                <div class="div-line"></div>

                <div class="title-description">
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Adipisci quibusdam magni iure facilis
                        omnis blanditiis expedita, porro repellendus! Deserunt minima praesentium quas commodi, optio
                        iste iusto odit sint fugiat laudantium!
                        Numquam aliquam earum illum qui fugiat aperiam similique perferendis consequatur saepe facere
                        minus, maxime dignissimos ad vel culpa sapiente ut blanditiis laborum illo dolore iste
                        repudiandae asperiores. Delectus, rem nulla!</p>
                </div>
            </div>


           

                <div class="row row-cols-4 mt-5">
                    <div class="col" v-for="card in cardList" :key="card.icon">
                        <!-- <div class="content"> -->
                        <i :class="card.icon"></i>
                        <div class="title-card"> {{ card.title }} </div>
                        <p class="card-info"> {{ card.info }} </p>
                    </div>
                </div>
            

<div class="br"></div>


            <div class="bg-curved">
                <div class="data d-flex justify-content-center">
                    <div v-for="data in dataList" :key="data.app">
                        <i :class="data.icon"></i>
                        <h3 class="number"> {{ data.number }} </h3>
                        <p class="data-info"> {{ data.info }} </p>
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
.bg-curved {

    background-image: url("/public/img/home-244125289.jpg");
    background-size: cover;
    min-height: 450px;

    .data{
        padding-top: 8rem;
    }
    
}

.br{
    width: 100%;
    height: 150px;
    /* border: 1px solid; */
    border-radius: 15%;
    position: relative;
    top: 45px;
    background: white;
    z-index: 2;
}

.br-after{
    top: -50px;

}





.data {
    padding-top: 8rem;
}
</style>