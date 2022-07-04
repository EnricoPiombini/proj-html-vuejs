<template>
    <div>
        <div class="jumbo-tron">
            <div class="jumbo-text text-center">
                <h1 class="fw-800">
                    BUILDING INSPIRING SPACES
                </h1>
                <h4 class="text-warning pb-4">
                    We Build Inspiring Commercial & ResIdential Spaces
                </h4>
                <div class="buttons d-flex justify-content-center g-4">
                    <div class="button">
                        <button type="button" class="my-btn btn-darker btn m-2 text-white">EXPLORE RECENT WORK</button>
                    </div>

                    <div class="button">
                        <button type="button" class="my-btn btn btn-warning m-2 ">GET A QUOTE TODAY</button>
                    </div>
                </div>
            </div>

        </div>
        <div class="banner-yellow bg-warning">
            <div class="banner-text text-center">
                <h2 class="pt-4">
                    Do You Have A Construction Project We Can Help With?
                </h2>
                <div class="button-offset">
                    <button type="button" class="my-btn btn btn-dark">GET A FREE QUOTE</button>

                </div>

            </div>

        </div>

    </div>

</template>


<script>
export default {

}


</script>


<style lang="scss" scoped>
@import "../assets/variables.scss";

.jumbo-tron {
    background-image: url("/public/img/home-slider-62528242.jpg");
    min-height: 550px;
    background-size: cover;
    object-fit: contain;

    .jumbo-text {
        padding-top: 10rem;
    }

    h1 {
        font-weight: 900;
        color: white;
        font-size: 60px;
    }

 .btn-darker {
        background-color: $btngray;
    }
}

.my-btn {
    padding: 1rem 2rem;
}

.banner-text {
    padding: 2rem;

    .button-offset {
        position: relative;
        top: 50px;
    }
}
</style>