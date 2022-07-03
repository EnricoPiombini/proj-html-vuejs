<template>
    <div>
        <div class="card custom-height">
            <img :src="article.img" class="card-img-top" alt="...">
            <div class="card-body">
                <h4 class="card-title">{{ article.subTitle }}</h4>
                <p class="card-text card-font">{{ article.text }}</p>

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

.card-body {

    .card-font {
        font-size: 18px;
    }
}


</style>