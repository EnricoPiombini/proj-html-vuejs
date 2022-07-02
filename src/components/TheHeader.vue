<template>
    <div>
        <nav class="mnav d-flex justify-content-between align-items-center p-4">
            <div class="left-side">
                <a class="navbar-brand" href="#">
                    <img src="img/construction_logo.png" class="d-inline-block align-text-top">
                </a>
            </div>
            <div class="right-side">
                <ul class="d-flex list-unstyled">
                    <li v-for="(link, i) in navLinks" :key="i">
                        <a class="navbar-brand fw-bold text-uppercase" :href="link.href"> {{ link.name }} </a>
                    </li>

                </ul>

            </div>
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
                    href: "#"
                },

            ]
        }
    }
}


</script>

<style lang="scss" scoped>
ul li a {
    margin: 1rem;
    font-size: 20px;
}
</style>