<template>
    <div>
        <div class="curve-div-top"></div>
        <div class="bg-curved">
            <div class="text text-center">
                <div class="section-title">
                    <h2 class="text-white">Our Home Owners Say</h2>
                </div>
                <div class="br"></div>

                <div class="img_section">
                    <img src="img/home-testimonial-113165296.jpg" alt="" srcset="" class="rounded-circle">
                </div>

                <div class="owners-text w-50 mt-4 m-auto">
                    <p class="font-italic text-white">
                        "No man but feels more of a man in the world if he have but a bit of ground that he can call his
                        own.
                        However small it is on the surface, it is four thousand mile deep and that in a very handsome
                        property"
                    </p>
                    <div class="owner-name">
                        <h5 class="text-white mt-4 fw-bold">
                            HARRY SMITH - NEW HOME OWNER
                        </h5>
                    </div>

                </div>

            </div>

        </div>
        <div class="curve-div-bottom"></div>

    </div>
</template>


<script>
export default {

}


</script>


<style lang="scss" scoped>
@import "../assets/variables.scss";

.bg-curved {
    background-image: url("/public/img/home-parallax-144609983.jpg");
    background-size: cover;
    min-height: 750px;

    .text {
        padding-top: 8rem;
    }

    .br {
        border: 1px solid;
        color: $primary;
        margin: auto;
        width: 200px;
        margin-bottom: 2rem;
        margin-top: 2rem;
    }
}

.curve-div-top {
    width: 100%;
    height: 150px;
    border-radius: 30%;
    position: relative;
    top: 100px;
    background:#F5F5F5;
    z-index: 2;
    transform: translateX(-50%);
    left: 50%;
}

.curve-div-bottom {
    width: 100%;
    height: 150px;
    border-radius: 30%;
    position: relative;
    bottom: 100px;
    background: #F5F5F5;
    z-index: 2;
    transform: translateX(-50%);
    left: 50%;
}

</style>