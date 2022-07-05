<template>
    <div>
        <div class="text text-center">
            <h2>Explore Recent Work</h2>
            <div class="br"></div>
            <p class="work-description m-auto w-50 mb-5">
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Similique ratione itaque assumenda laboriosam
                ducimus ipsa expedita odio fuga dicta blanditiis voluptatibus dolorum placeat.
            </p>
        </div>

        <div class="custom-padding">
            <div class="row justify-content-center g-3">
                <div class="col-sm-12 col-md-6 col-lg-6 col-xl-3" v-for="project in projectsList" :key="project.img">
                    <div class="content">
                        <img :src="project.img" alt="" class="w-100">
                    </div>

                </div>
            </div>
        </div>
        <div class="banner-projects d-flex align-items-center mt-5">
            <div class="br br-transparent"></div>
            <div>
                <h6 class="text-uppercase">View all Projects</h6>
            </div>
            <div class="br br-transparent"></div>



        </div>

    </div>

</template>


<script>
export default {
    data() {
        return {
            projectsList: [
                {
                    img: "img/project1-featured-294276386-400x400.jpg"
                },
                {
                    img: "img/project2-featured-15013609-400x400.jpg"
                },
                {
                    img: "img/project3-featured-189023420-400x400.jpg"
                }

            ]
        }

    }

}


</script>


<style lang="scss" scoped>
@import "../assets/variables.scss";

.br {
    border: 2px solid;
    color: $primary;
    margin: auto;
    width: 200px;
    margin-bottom: 2rem;
    margin-top: 2rem;
}

.br-transparent {
    color: $gray-200;
    flex-basis: 30%;
}

.custom-padding{
    padding: 2rem;
}
</style>