<template>
    <div>
        <div class="card custom-height" @mouseover="hover = true" @mouseleave="hover = false">
            <h4 class="bg-hover" v-if="hover">{{ article.subTitle }}</h4>
            <div v-else>
                <img :src="article.img" class="card-img-top" alt="...">
            </div>





            <div class="card-body">
                <h4 class="card-title pt-2 text-start">{{ article.subTitle }}</h4>
                <h6 class="date-year text-start">December 7th, 2015</h6>

                <p class="card-text my-card">{{ article.text }}</p>

                <!-- <div @mouseover="upHere = true" @mouseleave="upHere = false">
                    <h2> Something Something </h2>
                    <some-component v-show="upHere"></some-component>
                </div>
                on vue instance

                data : {
                upHere : false
                } -->




            </div>
        </div>



    </div>
</template>


<script>


export default {
    props: {
        article: Object

    },

    data() {
        return {
            hover: false
        }

    },
}




</script>


<style lang="scss" scoped>
@import "../assets/variables.scss";

.custom-height {
    height: 100%;
}

.card {
    .card-body {

        .my-card {
            font-size: 17px;
            text-align: start;
            padding: .5rem;
        }
    }
}

.bg-hover {
    &:hover {
        background-color: $primary;
        ;
    }
}
</style>