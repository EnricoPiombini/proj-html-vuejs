<template>
    <div>
        <div class="text text-center">
            <h4>
                Our Core Values
            </h4>
            <div class="br"></div>
            <p class="title-description">
                Lorem ipsum dolor sit amet consectetur, adipisicing elit. Maxime, ratione recusandae voluptate vel
                repellat neque harum autem fugit, similique eaque iure rerum, totam provident ducimus accusamus quaerat
                dolore. Ratione, voluptas.
            </p>
        </div>
        <div class="row">
            <div class="col-3" v-for="value in valuesList" :key="value.icon">
                <div class="content">
                    <i :class="value.icon"></i>
                    <h6 class="sub-title"> {{value.subTitle}} </h6>
                    <div class="div-line"></div>
                    <p class="text"> {{value.text}} </p>

                </div>

            </div>

        </div>



    </div>

</template>


<script>

export default {
    data() {
        return {
            valuesList: [
                {
                    icon: "fa-solid fa-house-chimney",
                    subTitle: "Great Services",
                    text: "Neque porro quisquiam est, qui dolorem ipsum quia dolor sit amet,consectetur,adipisci velit,sed quia"

                },

{
                    icon:"fa-solid fa-gear",
                    subTitle: "Highest Standard",
                    text: "Neque porro quisquiam est, qui dolorem ipsum quia dolor sit amet,consectetur,adipisci velit,sed quia"

                },
                {
                    icon:"fa-solid fa-users",
                    subTitle: "Professional Teams",
                    text: "Neque porro quisquiam est, qui dolorem ipsum quia dolor sit amet,consectetur,adipisci velit,sed quia"

                },
                {
                    icon:"fa-regular fa-lightbulb",
                    subTitle: "Creative Solutions",
                    text: "Neque porro quisquiam est, qui dolorem ipsum quia dolor sit amet,consectetur,adipisci velit,sed quia"

                },
            ]
        }
    }
}


</script>


<style lang="scss" scoped>
</style>