<template>
    <div>
        <div class="bg">

            <div class="row justify-content-center">
                <div class="col-12 col-sm-6 col-md-4">
                    <div class="content">
                        <div class="title">
                            <h2 class="text-white">Building Inspiring Spaces</h2>
                        </div>
                        <div class="br"></div>
                        <div class="section-description">
                            <p class="text-white">Vivamus sed consectetur tellus dolor sit amet, consectetur adipiscing
                                lorem elit sadip ipsum ets ficilis uns.
                            </p>
                        </div>
                    </div>
                </div>
                <div class="col-12 col-sm-6 col-md-4">
                    <div class="content">
                        <div class="button">
                            <button type="button" class="btn btn-warning">Warning</button>
                        </div>
                        <div class="info_section">
                            <p class="text-white mt-4"> Only takes a few seconds!</p>
                        </div>
                    </div>
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
.bg{
    background-image: url("/public/img/about-call-to-action-57862405.jpg");
    background-size: cover;
    padding: 7rem;
    
}
.br {
    border: 1px solid;
    color: $primary;
    margin: auto;
    width: 200px;
    margin-bottom: 2rem;
    margin-top: 2rem;
}
</style>