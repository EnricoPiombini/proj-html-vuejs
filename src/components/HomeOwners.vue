<template>
    <div>
        <div class="curve-div-top"></div>
<div>
        <div class="bg-curved">
            <div class="row justify-content-center">
                <div class="col-12">
                    <div class="slider">
                        <div class="section-title">
                            <h2 class="text-white">Our Home Owners Say</h2>
                        </div>
                        <div class="br"></div>

                        <div class="item">
                            <img :src="carouselList[currentIndex].img"
                                v-bind:alt="'Immagine di ' + carouselList[currentIndex].img" class="rounded-circle" />
                            <div class="text w-50 m-auto ">
                                <p class="text-white font-italic owner-statement">
                                    {{ carouselList[currentIndex].text }}
                                </p>

                                <div class="owners-name">
                                    <h5 class="fw-bold text-white">{{ carouselList[currentIndex].name }}</h5>

                                </div>
                            </div>
                        </div>

                        <div class="carousel-dots">
                            <button type="button" class="btn btn-outline-light btn-padding prev"
                                @click="changeImg('prev')"></button>
                            <button type="button" class="btn btn-outline-light btn-padding next"
                                @click="changeImg('next')"></button>
                        </div>



                    </div>

                </div>
            </div>


            <!-- 
            <div class="slidesInfo slides-index" v-for="(slider, i) in carouselList" :key="i"
                :class="{ 'display-none': slider.id===1 }">
                <div class="text text-center">
                    <div class="section-title">
                        <h2 class="text-white">Our Home Owners Say</h2>
                    </div>
                    <div class="br"></div>

                    <div class="img_section">
                        <img :src="slider.img" alt="" srcset="" class="rounded-circle">
                    </div>

                    <div class="owners-text w-50 mt-4 m-auto">
                        <p class="font-italic text-white">
                            {{ slider.text }}
                        </p>
                        <div class="owner-name">
                            <h5 class="text-white mt-4 fw-bold">
                                {{ slider.name }}
                            </h5>
                        </div>

                    </div>

                </div>
            </div> -->

        </div>
</div>
        <!-- <div class="carousel-dots">
            <button type="button" class="btn btn-outline-light btn-padding prev" @click="changeImg('prev')"></button>
            <button type="button" class="btn btn-outline-light btn-padding next" @click="changeImg('next')"></button>
        </div> -->

        <div class="curve-div-bottom"></div>


    </div>
</template>


<script>
export default {
    data() {
        return {
            currentIndex: 0,
            carouselList: [
                {
                    img: "img/home-testimonial-113165296.jpg",
                    text: "No man but feels more of a man in the world if he have but a bit of ground that he can call his own However small it is on the surface, it is four thousand mile deep and that in a very handsome property",
                    name: "HARRY SMITH - NEW HOME OWNER"

                },
                {
                    img: "img/home-testimonial-84268399.jpg",
                    text: "No man but feels more of a man in the world if he have but a bit of ground that he can call his own However small it is on the surface, it is four thousand mile deep and that in a very handsome property",
                    name: "JOHN DOE - PROPERTY INVESTOR",


                }
            ]
        }
    },
    methods: {
        changeImg(direction) {
            if (direction === "next") {
                this.currentIndex++;


                if (this.currentIndex >= this.carouselList.length) {
                    this.currentIndex = 0;
                }
            } else if (direction === 'prev') {
                this.currentIndex--

                if (this.currentIndex < 0) {
                    this.currentIndex = this.carouselList.length - 1;
                }
            }

        }

    }
}

</script>


<style lang="scss" scoped>
@import "../assets/variables.scss";

.bg-curved {
    background-image: url("/public/img/home-parallax-144609983.jpg");
    background-size: cover;
    min-height: 960px;
    position: relative;

    .slider {
        padding-top: 10rem;
    }

    .text {
        padding-top: 3rem;
        position: relative;
    }

    .br {
        border: 1px solid;
        color: $primary;
        margin: auto;
        width: 200px;
        margin-bottom: 2rem;
        margin-top: 2rem;
    }
}

.curve-div-top {
    width: 100%;
    height: 150px;
    border-radius: 30%;
    position: relative;
    top: 100px;
    background: #F5F5F5;
    z-index: 2;
    transform: translateX(-50%);
    left: 50%;
}

.carousel-dots {
    position: relative;
    top: 20px;

    .btn-padding {
        padding: 0.3rem;
        margin: .5rem;
    }

}


.curve-div-bottom {
    width: 100%;
    height: 150px;
    border-radius: 30%;
    position: relative;
    bottom: 100px;
    background: #F5F5F5;
    z-index: 2;
    transform: translateX(-50%);
    left: 50%;
}

.display-none {
    display: none;
}
</style>