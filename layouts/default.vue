<template>
  <div>
    <!-- <Header /> -->
    <TheHeader @sidenavToggle='displaySidenav = !displaySidenav' /> 
    <TheSidenav :show="displaySidenav" @close="displaySidenav = false" /> 
    <Nuxt />
  </div>
</template>

<script>
import Header from '@/components/Header.vue'
import TheHeader from '@/components/Navigation/TheHeader'
import TheSidenav from '@/components/Navigation/TheSidenav'
export default {
    components :{
      Header,
      TheHeader,
      TheSidenav
    },
    data(){
      return {
        displaySidenav : false
      }
    }
    
}
</script>

<style>
html {
font-family: 'Open Sans', sans-serif;
}
body {
  margin:0
}
</style>
