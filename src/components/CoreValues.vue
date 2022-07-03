<template>
    <div>
        <div class="bg mt-5">
            <div class="text text-center pt-5">
                <h2>
                    Our Core Values
                </h2>
                <div class="br"></div>
                <p class="title-description m-auto w-50 mb-5">
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Similique ratione itaque assumenda
                    laboriosam
                    ducimus ipsa expedita odio fuga dicta blanditiis voluptatibus dolorum placeat.
                </p>
            </div>
            <div class="row">
                <div class="col-3" v-for="(value, i) in valuesList" :key="i">
                    <div class="content">
                        <div :class="{
                            'bg-red': value.id === 1,
                            'bg-blue': value.id === 2,
                            'bg-orange': value.id === 3,
                            'bg-light-green': value.id === 4, }"
                            id="bg-icon">
                            
                            <i id="value_color" :class="value.icon"></i>
                        </div>

                        <h6 class="sub-title"> {{ value.subTitle }} </h6>
                        <div class="div-line"></div>
                        <p class="text"> {{ value.text }} </p>

                    </div>

                </div>

            </div>
        </div>
    </div>
</template>


<script>

"{'bg-red': value.id === 1}"

export default {
    data() {
        return {


            valuesList: [
                {
                    icon: "fa-solid fa-house-chimney",

                    subTitle: "Great Services",
                    text: "Neque porro quisquiam est, qui dolorem ipsum quia dolor sit amet,consectetur,adipisci velit,sed quia",
                    id: 1


                },

                {
                    icon: "fa-solid fa-gear",
                    subTitle: "Highest Standard",
                    text: "Neque porro quisquiam est, qui dolorem ipsum quia dolor sit amet,consectetur,adipisci velit,sed quia",
                    id: 2
                },
                {
                    icon: "fa-solid fa-users",
                    subTitle: "Professional Teams",
                    text: "Neque porro quisquiam est, qui dolorem ipsum quia dolor sit amet,consectetur,adipisci velit,sed quia",
                    id: 3
                },
                {
                    icon: "fa-regular fa-lightbulb",
                    subTitle: "Creative Solutions",
                    text: "Neque porro quisquiam est, qui dolorem ipsum quia dolor sit amet,consectetur,adipisci velit,sed quia",
                    id: 4

                },
            ],

            computed: {


            }
        }
    }
}


</script>


<style lang="scss" scoped>
@import "../assets/variables.scss";

.bg {
    background-color: #F5F5F5
}

;

.br {
    border: 2px solid;
    color: $primary;
    margin: auto;
    width: 200px;
    margin-bottom: 2rem;
    margin-top: 2rem;
}

.content {

    #bg-icon {

        box-sizing: content-box;
        height: 120px;
        width: 120px;
        line-height: 120px;
        border-radius: 50%;

        font-size: 70px;
        margin: auto;
    }

    i {
        color: $gray-200
    }
}

.bg-red {
    background-color: #4EA4A5;
}

.bg-blue {
    background-color: #4E6DA5;
}

.bg-orange {
    background-color: #F6722A;
}

.bg-light-green {
    background-color: #A7CF47;
}
</style>