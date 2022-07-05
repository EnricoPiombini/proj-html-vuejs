<template>
    <div>
        <TheJumbo></TheJumbo>
        <TheSpecialists></TheSpecialists>
        <RecentWork></RecentWork>
        <CoreValues></CoreValues>
        <HomeOwners></HomeOwners>


        <div class="bg-relative">
            <div class="text text-center pt-5">
                <div class="section-title">
                    <h2>Latest News</h2>
                </div>
                <div class="br"></div>
                <div class="section-description w-50 m-auto">
                    <p class="font">Lorem ipsum dolor sit amet consectetur adipisicing elit. Magnam aliquid quis
                        aspernatur amet,
                        expedita repellat, consequatur nisi distinctio quibusdam voluptatem facilis. Veniam quas
                        soluta
                        distinctio quasi doloremque molestias, est nostrum!</p>
                </div>


                <div class="row justify-content-center g-3">
                    <div class="col-12 col-sm-12 col-md-6 col-lg-3" v-for="article in articleList" :key="article.img">
                        <TheLatests :article="article"></TheLatests>
                    </div>
                </div>

                <div class="banner-projects d-flex align-items-center mt-5 pb-5">
                    <div class="br br-transparent"></div>
                    <div>
                        <h6 class="text-uppercase">View all Articles</h6>
                    </div>
                    <div class="br br-transparent"></div>
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
                    text: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Magnam aliquid quis aspernatur amet, consectetur adisciping elit.Vivamus purus nisl elementum vitae consequat at tristique ut enim. Sed ut dignissim leo.Nullam sed metus id sapien faucibus rhoncus sed."



                },
                {
                    img: "img/blog-post-92486644-400x241.jpg",
                    subTitle: "How We Manage Large Construction Projects",
                    text: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Magnam aliquid quis aspernatur amet, consectetur adisciping elit.Vivamus purus nisl elementum vitae consequat at tristique ut enim. Sed ut dignissim leo.Nullam sed metus id sapien faucibus rhoncus sed."

                },
                {
                    img: "img/blog-post-332773904-400x241.jpg",
                    subTitle: "Future proofing a modern home",
                    text: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Magnam aliquid quis aspernatur amet, consectetur adisciping elit.Vivamus purus nisl elementum vitae consequat at tristique ut enim. Sed ut dignissim leo.Nullam sed metus id sapien faucibus rhoncus sed."

                }
            ]


        }
    }
}


</script>


<style lang="scss" scoped>
@import "../assets/variables.scss";
.bg-relative {
    background-color: #F5F5F5;
    position: relative;
    bottom: 140px;
}

.font {
    font-size: 17px;
}

.br{
    border: 2px solid;
    color: $primary;
    margin: auto;
    width: 200px;
    margin-bottom: 2rem;
    margin-top: 2rem;
}

.br-transparent{
    color: $gray-100;
    flex-basis: 30%;
}
</style>