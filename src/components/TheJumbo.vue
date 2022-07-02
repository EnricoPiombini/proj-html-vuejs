<template>
    <div>
        <div class="jumbo-tron">
            <div class="jumbo-text text-center">
                <h1>
                    BUILDING INSPIRING SPACES
                </h1>
                <h4>
                    We Build Inspiring Commercial & ResIdential Spaces
                </h4>
                <div class="buttons d-flex justify-content-center g-4">
                    <div class="button">
                        <button type="button" class="btn btn-secondary">Secondary</button>
                    </div>

                    <div class="button">
                        <button type="button" class="btn btn-warning">Warning</button>
                    </div>
                </div>
            </div>

        </div>
        <div class="banner-yellow bg-warning">
            <div class="banner-text text-center">
                <h2>
                    Do You Have A Construction Project We Can Help With?
                </h2>
                <div class="button-offset">
                    <button type="button" class="btn btn-dark">Dark</button>

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
.jumbo-tron {
    background-image: url("/public/img/home-slider-62528242.jpg");
    min-height: 550px;
    background-size: cover;
    object-fit: contain;

    .jumbo-text {
        padding-top: 10rem;
    }
}

.banner-text {
padding: 2rem;

    .button-offset {
        position: relative;
        top: 50px;
    }
}
</style>