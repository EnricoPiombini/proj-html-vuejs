<template>
  <div id="app">

<TheHeader></TheHeader>


<TheMain></TheMain>


<TheFooter></TheFooter>


  </div>
</template>

<script>
import TheHeader from './components/TheHeader.vue';
import TheFooter from './components/TheFooter.vue';
import TheMain from './components/TheMain.vue';


export default {
   
    components: { TheHeader, TheFooter, TheMain }
}

</script>

<style lang="scss">
@import "./assets/main.scss";



#app {
  font-family: 'Raleway', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  letter-spacing: 0.04rem;
  
 
}
</style>
