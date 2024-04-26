<template>
  <NavBar/>
  <HeroSection/>
  <BrandsComponent/>
</template>

<script>
import NavBar from './components/NavBar.vue'
import HeroSection from './components/HeroSection.vue'
import BrandsComponent from './components/BrandsComponent.vue'

export default {
  name: 'App',
  components: {
    NavBar,
    HeroSection,
    BrandsComponent
  }
}
</script>

