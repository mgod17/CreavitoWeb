<template>
    <div class="contenedor-discos hidden laptop:block ">
      <img src="../assets/klipartz.com.png" alt="Logo" class="disco">
      <div class="absolute top-12 left-36 w-44 h-80 bg-gray-300 overflow-hidden z-[-10]">
      <div class="p-5 border-b border-gray-300 text-lg">Flyers</div>
      <div class="p-5 border-b border-gray-300 text-lg">Videos</div>
      <div class="p-5 border-b border-gray-300 text-lg">Paginas Webs</div>
    </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'DiscoSection',
  };
  </script>
  
  <style scoped>

  .contenedor-discos {
    width: auto; 
    height: auto; 
    position: relative; 
    top: 80px;
    left:100px;
    overflow: visible;
     animation:  2s infinite alternate, balanceo 5s infinite; 
  }
  .disco {
    width: 367px;
    height: 526px;
    background-size: cover;
    background-position: center;
    position: absolute;
    border-bottom-left-radius: 50%;
  }
  @keyframes balanceo {
  0% {
    transform: rotateZ(0) translateX(0);
  }
  50% {
    transform: rotateZ(-5deg) translateX(-10px);
  }
  100% {
    transform: rotateZ(0) translateX(0);
  }
}
 
  
  </style>
  