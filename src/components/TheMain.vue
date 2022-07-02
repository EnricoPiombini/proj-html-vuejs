<template>
<div>
<TheJumbo></TheJumbo>
<TheSpecialists ></TheSpecialists>
<RecentWork></RecentWork>
<CoreValues></CoreValues>
<HomeOwners></HomeOwners>
<TheLatests></TheLatests>
<TrustedPartners></TrustedPartners>
<BuildingSpaces></BuildingSpaces>

</div>

</template>


<script>
import TheJumbo from "./TheJumbo.vue";
import TheSpecialists from "./TheSpecialists.vue";
import RecentWork from "./RecentWork.vue";
import CoreValues from "./CoreValues.vue";
import HomeOwners from "./HomeOwners.vue";
import TheLatests from "./TheLatests.vue";
import TrustedPartners from "./TrustedPartners.vue";
import BuildingSpaces from "./BuildingSpaces.vue";

export default{


    components: { TheJumbo, TheSpecialists, RecentWork, CoreValues, 
    HomeOwners, TheLatests, TrustedPartners, BuildingSpaces }
}


</script>


<style lang="scss" scoped>



</style>