<template>
  <DiscoSection/>
  <div class="GradientBackground bg-fixed "></div>
  <div class=" pt-32 h-screen flex flex-col justify-between">
    <div class="container  mx-auto text-end pt-20 pr-10">
      <h1 class="text-5xl text-white font-bold mb-8">¡Destaca en el mundo digital!</h1>
      <button class="bg-yellow-500 hover:bg-yellow-600 text-white font-bold py-2 px-4 rounded">Ver Casos de éxito</button>
    </div>
  </div>
</template>

<script>
import DiscoSection from './DiscosSection.vue'

export default {
  name: 'HeroSection',
  components: {
    DiscoSection
  }
};
</script>
<style scoped>
.GradientBackground {
  width: 400%; 
  height: 100%; 
  position: absolute;
  left: 0;
  top: 0;
  z-index: -1;
  --gradientColorZero: #0c0c0c;
  --gradientColorOne: #e9c307;
  --gradientColorTwo: #c3bb6e;
  --gradientColorThree: #302f30;
  --gradientColorZeroTransparent: rgba(169, 96, 238, 0);
  --gradientColorOneTransparent: rgba(255, 51, 61, 0);
  --gradientColorTwoTransparent: rgba(144, 224, 255, 0);
  --gradientColorThreeTransparent: rgba(255, 203, 87, 0);
  background: radial-gradient(var(--gradientColorZero) 40%, var(--gradientColorTwoTransparent) 60%) -620px -180px no-repeat, radial-gradient(var(--gradientColorThree) 33%, var(--gradientColorThreeTransparent) 67%) -120px -24px no-repeat, radial-gradient(var(--gradientColorTwo) 40%, var(--gradientColorTwoTransparent) 70%) -470px 150px no-repeat, var(--gradientColorZero);
  background-size: 100vw 100vh; 

}

</style>