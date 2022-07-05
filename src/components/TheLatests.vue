<template>
    <div>
        <div class="card custom-height">
            <img :src="article.img" class="card-img-top" alt="...">
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

        }

    }
}



</script>


<style lang="scss" scoped>
@import "../assets/variables.scss";

.custom-height {
    height: 100%;
}

.card {

    &:hover {
        background-color: $primary;
        ;
    }

    .card-body {

        .my-card {
            font-size: 17px;
            text-align: start;
            padding: .5rem;
        }
    }
}
</style>