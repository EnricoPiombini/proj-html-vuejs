<template>
    <div>
        <div class="top_img">
            <img :src="article.img" alt="">
        </div>
        <div class="sub-title">
            <h4> {{ article.subTitle }} </h4>
        </div>
        <div class="article-text">
            <p class="text">
                {{ article.text }}

            </p>
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
</style>