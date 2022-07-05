<template>
    <div>
        <div class="card custom-height p-3" @mouseover="hover = true" @mouseleave="hover = false">

            <div class="content">


                <div class="card bg-hover p-3" v-if="hover">
                    <div class="content-else">
                        <div class="icon">
                            <i class="fa-solid fa-magnifying-glass "></i>
                            <i class="fa-solid fa-link "></i>
                        </div>
                        <h5 class="text-white">{{ article.subTitle }}</h5>
                        <div>
                            <h6 class="text-white">Architecture, Buildings, Construction, News</h6>
                        </div>
                    </div>
                </div>

                <div v-else>
                    <img :src="article.img" class="card-img-top" alt="...">
                </div>

            </div>




            <div class="card-body">
                <h4 class="card-title pt-2 text-start">{{ article.subTitle }}</h4>
                <h6 class="date-year text-start">December 7th, 2015</h6>

                <p class="card-text my-card">{{ article.text }}</p>

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

.icon {


    i {
        font-size: 20px;
        border: 1px solid;
        border-radius: 50%;
        padding: 1rem;
        color: $primary;
        background-color: white;
        
}

}
.bg-hover {
    &:hover {
        background-color: $primary;
        ;
    }
}
</style>