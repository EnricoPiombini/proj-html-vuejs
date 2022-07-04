<template>
    <div>
        <BuildingSpaces></BuildingSpaces>

        <div class="br"></div>
            <div class="bg">
                <div class="row">
                    <div class="col-12 col-sm-6 col-md-3">
                        <div class="content p-4">
                            <div class="logo_footer mb-3 text-start">
                                <img src="img/footer-logo.png" alt="">
                            </div>
                            <div class="description_logo">
                                <p>We are specialist in the construction of unique and exclusive properties.
                                    Our work isnpires. We pride ourselves amd delivering outstanding quality and design
                                    for leading clients across the world.
                                </p>

                            </div>
                            <div class="button">
                                <button type="button" class="btn btn-warning">LEARN MORE</button>
                            </div>

                        </div>
                    </div>
                    <div class="col-12 col-sm-6 col-md-3">
                        <div class="content p-4">
                            <div class="col_title">
                                <h5 class="text-warning text-start fw-bold mb-5">LATEST TWEETS</h5>
                            </div>
                            <div class="social_tweet">
                                <div class="profile d-flex justify-content-between">
                                    <div class="logo_small d-flex">
                                        <div>
                                            <img src="img/3a74ce3d0532b7773b174c45ca3bd05a_normal.png" alt="">
                                        </div>
                                        <div>
                                            <h5>ThemeFusion</h5>
                                            <h6>@Theme_Fusion</h6>
                                        </div>
                                    </div>

                                    <div class="social_logo">
                                        <i class="fa-brands fa-twitter"></i>
                                    </div>

                                </div>
                                <div class="tweet-content">
                                    <p class="text-white">Do you need sublime WordPress hosting for your next webite?
                                        Take advantage of exclusive partners offers that we secured just for you,
                                        & launch your site in seconds with <a href="">#avada</a> on WP Engine hosting
                                        & get 30% Off this Black Friday <a href="">bit.ly/3kjLLE2#BlackFriday2020</a>
                                    </p>
                                </div>

                                <div class="footer_img">
                                    <img src="img/En2TRxLW4AEiWUN.jpeg" alt="" class="w-100">
                                </div>

                                <div class="footer_icon d-flex justify-content-between">
                                    <div class="icon-left">
                                        <i class="fa-regular fa-heart"></i>
                                        <i class="fa-solid fa-arrow-right-from-bracket"></i>
                                    </div>
                                    <div class="post_time">
                                        <p>22h</p>
                                    </div>


                                </div>



                            </div>
                        </div>
                    </div>

                    <ContactUs></ContactUs>

                    <div class="col-12 col-sm-6 col-md-3">
                        <div class="content p-4">
                            <div class="col-title">
                            <h5 class="text-warning text-start fw-bold mb-5">FIND US</h5>
                            </div>
                        <div class="img_map">
                            <img src="img/construction_map_pin.png-Notti" alt="" class="w-100">
                        </div>
                        </div>
                    </div>
                </div>
            </div>

<div class="bg-banner">
    <div class="text text-start">
        <p>COPYRIGHT 2012-2015 AVADA THEME FUSION | ALL RIGHTS RESERVED | POWERED BY WORDPRESS </p>
    </div>
</div>
        
    </div>
</template>


<script>
import BuildingSpaces from "./BuildingSpaces.vue";
import ContactUs from "./ContactUs.vue";

export default {

    components: {
        BuildingSpaces,
        ContactUs
    },

    data() {
        return {

        }
    }


}

</script>

<style lang="scss" scoped>
@import "../assets/variables.scss";

.bg{
    background-color:#1E1E1E;
    color: #565656;
}

.bg-banner{
background-color: #111111;
padding: 2rem;
}

</style>