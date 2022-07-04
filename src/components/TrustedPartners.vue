<template>
    <div>
        <div class="text text-center">
            <div class="section-title">
                <h2>Trusted Partners</h2>
            </div>
            <div class="br"></div>
            <div class="section-description">
                <p class="m-auto w-50 mb-5">Lorem ipsum dolor sit amet consectetur adipisicing elit. Cum dolorum eius id
                    totam autem quis a velit
                    voluptate doloremque molestiae, reprehenderit quasi quae beatae ipsa assumenda magni. Modi, minus!
                    Facilis?</p>
            </div>
        </div>

        <div class="row justify-content-center align-items-center mb-5">
            <div class="col-12 col-sm-6 col-md-2" v-for="partners in partnersList" :key="partners.img">
                <div class="content">
                    <div class="partners_logo">
                        <img :src="partners.img" alt="" class="w-100">
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
@import "../assets/variables.scss";

.br {
    border: 1px solid;
    color: $primary;
    margin: auto;
    width: 200px;
    margin-bottom: 2rem;
    margin-top: 2rem;
}
</style>