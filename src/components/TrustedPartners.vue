<template>
    <div>
        <div class="text text-center">
            <div class="section-title">
                <h4>Trusted Partners</h4>
            </div>
            <div class="br"></div>
            <div class="section-description">
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Cum dolorum eius id totam autem quis a velit
                    voluptate doloremque molestiae, reprehenderit quasi quae beatae ipsa assumenda magni. Modi, minus!
                    Facilis?</p>
            </div>
        </div>

        <div class="row justify-content-center">
            <div class="col-2" v-for="partners in partnersList" :key="partners.img">
                <div class="content">
                    <div class="partners_logo">
                        <img :src="partners.img" alt="">
                    </div>
                </div>
            </div>
        </div>

    </div>

</template>


<script>
export default {
    data() {
        return {
            partnersList: [
                {
                    img: "img/home-logo11-219096700-320x202.png"
                },
                {
                    img: "img/home-logo10-219096700-320x202.png"
                },
                 {
                    img: "img/home-logo9-219096700-320x202.png"
                },
                 {
                    img: "img/home-logo2-219096700-320x202.png"
                },
                 {
                    img: "img/home-logo1-219096700-320x202.png"
                },
            ]
        }
    }
}


</script>


<style lang="scss" scoped>
</style>