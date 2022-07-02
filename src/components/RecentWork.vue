<template>
    <div>
        <div class="text text-center">
            <h4>Explore Recent Work</h4>
            <div class="br"></div>
            <p class="work-description">
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Similique ratione itaque assumenda laboriosam
                ducimus ipsa expedita odio fuga dicta blanditiis voluptatibus dolorum placeat enim quasi culpa deserunt
                corporis, omnis fugit.

            </p>
        </div>
        <div class="row row-cols-4 justify-content-center">
            <div class="col" v-for="project in projectsList" :key="project.img">
                <div class="content">
                    <img :src="project.img" alt="">
                </div>

            </div>
        </div>

<div class="banner-projects">
    <h6>View all Projects</h6>
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
</style>