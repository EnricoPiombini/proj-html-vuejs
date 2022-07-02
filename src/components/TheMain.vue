<template>
    <div>
        <TheJumbo></TheJumbo>
        <TheSpecialists></TheSpecialists>
        <RecentWork></RecentWork>
        <CoreValues></CoreValues>
        <HomeOwners></HomeOwners>

        <div>

            <div class="text text-center">
                <div class="section-title">
                    <h4>Latest News</h4>
                </div>
                <div class="br"></div>
                <div class="section-desctiption">
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Magnam aliquid quis aspernatur amet,
                        expedita repellat, consequatur nisi distinctio quibusdam voluptatem facilis. Veniam quas
                        soluta
                        distinctio quasi doloremque molestias, est nostrum!</p>
                </div>


                <div class="row row-cols-3 justify-content-center">
                   
                    <div class="col" v-for="article in articleList" :key="article.img">
                        <div class="content">
                             <TheLatests :article="article"></TheLatests>
                        </div>
                    </div>
                </div>

            </div>


        </div>

        <TrustedPartners></TrustedPartners>



    </div>
</template>


<script>
import TheJumbo from "./TheJumbo.vue";
import TheSpecialists from "./TheSpecialists.vue";
import RecentWork from "./RecentWork.vue";
import CoreValues from "./CoreValues.vue";
import HomeOwners from "./HomeOwners.vue";
import TheLatests from "./TheLatests.vue";
import TrustedPartners from "./TrustedPartners.vue";


export default {




    components: {
        TheJumbo, TheSpecialists, RecentWork, CoreValues,
        HomeOwners, TheLatests, TrustedPartners
    },

    data() {
        return {
            articleList: [
                {
                    img: "img/blog-post-134132600-400x241.jpg",
                    subTitle: "Redeveloping Florida's Remote Southern Coast",
                    text: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Magnam aliquid quis aspernatur amet",

                },
                {
                    img: "img/blog-post-92486644-400x241.jpg",
                    subTitle: "How We Manage Large Construction Projects",
                    text: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Magnam aliquid quis aspernatur amet",

                },
                {
                    img: "img/blog-post-332773904-400x241.jpg",
                    subTitle: "Future proofing a modern home",
                    text: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Magnam aliquid quis aspernatur amet",

                }
            ]


        }
    }
}


</script>


<style lang="scss" scoped>
</style>