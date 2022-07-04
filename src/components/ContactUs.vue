<template>
    
        <div class="col-12 col-sm-6 col-md-3">
            <div class="content p-4">
                <h5 class="text-warning fw-bold text-start mb-5">CONTACT US</h5>
                <div class="contact-List">
                 <div class="d-flex" v-for="contact in contactsList" :key="contact.icon">
                    <div class="icon">
                        <i :class="contact.icon"></i>
                    </div>
                    <div class="address">
                        <p>{{contact.address}}</p>
                    </div>
                 </div>
                   
                </div>
            </div>

        </div>
 

</template>

<script>
export default {
    data() {
        return {
            contactsList: [
                {
                    icon: "fa-solid fa-globe",
                    address:"Corporate Location 1600 Amphitheatre Parkway London WC11BA"
                },
                {
                    icon: "fa-solid fa-house-chimney",
                    address: "Residential Location 9521 Broadsberry Avenue Paddington RC7 9ZA"
                },
                {
                    icon: "fa-solid fa-phone-flip",
                    address: "1.800.458.556 / 1.800.535.2112"
                },
                {
                    icon: "fa-regular fa-envelope",
                    address: "info@your-domain.com"
                },
                {
                    icon: "fa-regular fa-clock",
                    address: "Monday-Friday: 9:00 AM - 6:00 PM"
                },
                {
                    icon: "fa-regular fa-clock",
                    address:"Saturday-Sunday: 9:00 AM - 12:00 PM"
                },
            ]
        }
    }
}

</script>

<style lang="scss" scoped>
@import "../assets/variables.scss";
</style>