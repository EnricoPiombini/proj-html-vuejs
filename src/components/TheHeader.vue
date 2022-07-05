<template>
    <div>
        <nav class="navbar p-3 fixed-top navbar-expand-lg navbar-light bg-light justify-content-between">
            <div class="left-side">
                <a class="navbar-brand" href="#">
                    <img src="img/construction_logo.png" class="d-inline-block align-text-top">
                </a>
            </div>

            <div class="right-side d-flex align-items-center">
                <div class="collapse navbar-collapse" id="navbarTogglerDemo02">

                    <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                        <li class="nav-item" v-for="(link, i) in navLinks" :key="i">
                            <div :class="{'my-btn': link.id===1}">
                                <a class="nav-link fw-bold text-uppercase" :href="link.href"> {{ link.name }} </a>
                            </div>
                        </li>

                    </ul>
                </div>
            </div>

            <button class="navbar-toggler bg-warning text-white" type="button" data-bs-toggle="collapse"
                data-bs-target="#navbarTogglerDemo02" aria-controls="navbarTogglerDemo02" aria-expanded="false"
                aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
        </nav>
    </div>
</template>






<script>

export default {
    name: "TheNavbar",
    data() {
        return {
            navLinks: [
                {
                    name: "Home",
                    href: "#"
                },
                {
                    name: "About",
                    href: "#"
                },
                {
                    name: "Services",
                    href: "#"
                },
                {
                    name: "Work",
                    href: "#"
                },
                {
                    name: "Articles",
                    href: "#"
                },
                {
                    name: "Get Quote",
                    href: "#",
                    id: 1
                },

            ]
        }
    }
}


</script>

<style lang="scss" scoped>
@import "../assets/variables.scss";

ul li a {
    margin: 1rem;
    font-size: 16px;
    color: $silver;


    &:hover {
        color: $primary;
    }
}

.my-btn {
    background: $primary;
    padding-left: 1rem;
    padding-right: 1rem;
}
</style>