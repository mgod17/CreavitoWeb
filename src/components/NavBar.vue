<template>
  <div>
    <div
      class="absolute bg-white border-b border-gray-300 z-10 top-20 left-0 right-0 mt-4 flex flex-col justify-center items-center"
      :class="{ 'hidden': !showMenu, 'md:block': showMenu }">
      <a href="#" class="block font-bold pt-20 pb-10 px-4 text-black hover:text-gray-400">Inicio</a>
      <a href="#" class="block font-bold py-10 px-4 text-black hover:text-gray-400">Servicios</a>
      <a href="#" class="block font-bold py-10 px-4 text-black hover:text-gray-400">Proyectos</a>
      <a href="#" class="block font-bold py-10 pb-14 px-4 text-black hover:text-gray-400">Contacto</a>
    </div>
    <nav class="bg-black z-10 top-0 left-0 right-0 flex flex-col justify-center items-center fixed w-full">
      <div class="container mx-auto px-6">
        <div class="flex justify-between items-center ">
          <div>
            <img src="../assets/LogoNavbar1.svg" alt="Logo" class="h-16">
          </div>
          <div class="hidden laptop:flex  px-8 py-2 rounded items-center space-x-20">
            <a href="#" class="text-white text-lg font-bold hover:text-gray-400">Inicio</a>
            <a href="#" class="text-white text-lg font-bold hover:text-gray-400">Servicios</a>
            <a href="#" class="text-white text-lg font-bold hover:text-gray-400">Proyectos</a>
            <a href="#" class="text-white text-lg font-bold hover:text-gray-400">Contacto</a>
          </div>
          <div class="laptop:hidden">
            <div class="mr-5 block cursor-pointer" @click="toggleMenu">
              <span class="block w-6 h-0.5 bg-white my-1 transform transition duration-300"
                :class="{ 'rotate-45 translate-y-3': showMenu, '-rotate-1 -translate-y-0': !showMenu }"></span>
              <span class="block w-6 h-0.5 bg-white my-1 transform transition duration-300"
                :class="{ 'opacity-0': showMenu }"></span>
              <span class="block w-6 h-0.5 bg-white my-1 transform transition duration-300"
                :class="{ '-rotate-45 translate-y-0': showMenu, 'rotate-1 translate-y-0': !showMenu }"></span>
            </div>

          </div>
        </div>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  name: 'NavBar',
  data() {
    return {
      showMenu: false
    };
  },
  methods: {
    toggleMenu() {
      this.showMenu = !this.showMenu;
    }
  }
}
</script>
