<template>
  <!-- Navbar -->
  <nav class="flex bg-green-50 shadow-md font-bold text-lg items-center fixed w-full m-0 p-0 top-0">
    <img src="../assets/rdev.svg" alt="" class="h-20 w-20 m-2">
    <a href="javascript:void(0)"
      class="py-2 px-4 bg-clip-text bg-gradient-to-tr from-green-300 via-green-400 to-blue-500 text-transparent transition duration-500 transform scale-95 hover:scale-105 hidden md:block">
      About Me
    </a>
    <a href="javascript:void(0)"
      class="py-2 px-4 bg-clip-text bg-gradient-to-tr from-green-300 via-green-400 to-blue-500 text-transparent transition duration-500 transform scale-95 hover:scale-105 hidden md:block">
      Git Contributions
    </a>
    <a href="javascript:void(0)"
      class="py-2 px-4 bg-clip-text bg-gradient-to-tr from-green-300 via-green-400 to-blue-500 text-transparent transition duration-500 transform scale-95 hover:scale-105 hidden md:block">
      Gallery
    </a>
    <a href="javascript:void(0)"
      class="py-2 px-4 bg-clip-text bg-gradient-to-tr from-green-300 via-green-400 to-blue-500 text-transparent transition duration-500 transform scale-95 hover:scale-105 ml-auto hidden md:block">
      <i class="lni lni-lg lni-enter"></i>
      Login
    </a>
    <a href="javascript:void(0)"
      class="py-2 px-4 text-white bg-gradient-to-tr from-green-300 via-green-400 to-blue-500 text-transparent transition duration-50 transform scale-95 hover:scale-105 ml-auto block md:hidden rounded-md mr-2 shadow-lg">
      <i class="lni lni-lg lni-menu"></i>
    </a>
  </nav>
  <!-- Navbar End -->
  <!-- Container -->
  <div class="container my-32 mx-auto">
    <div class="bg-green-50 mx-2 px-1 py-1 rounded-md shadow-md">
      <!-- About Me -->
      <div
        class="bg-clip-text bg-gradient-to-tr from-green-300 via-green-400 to-blue-500 text-transparent italic text-justify flow-root">
        <h1 class="font-bold py-3 px-2 text-lg">My name is {{msg}}</h1>
        <img src="../assets/RickyCaesarAprillaTiaka.jpg"
          class="float-none mx-auto my-5 sm:my-5 md:my-0 lg:my-0 md:float-right md:mx-5 lg:float-right rounded-lg shadow-lg h-96" alt="">
        <p class="px-2 font-semibold">{{msg2}}</p>
      </div>
      <!-- About Me end -->
      <!-- Github Contributions -->
      <div class="bg-clip-text bg-gradient-to-tr from-green-300 via-green-400 to-blue-500 text-transparent italic">
        <h1 class="font-bold py-3 px-2 text-lg">My Contributions in the last year</h1>
        <p class="px-2 font-semibold">- Github -</p>
      </div>
      <img class="mx-auto" src="https://ghchart.rshah.org/39d59c/RickyCaesarAprillaTiaka"
        alt="RickyCaesarAprillaTiaka's Github chart" />
      <!-- Github Contributions End -->
      <!-- Github Contributions -->
      <div class="bg-clip-text bg-gradient-to-tr from-green-300 via-green-400 to-blue-500 text-transparent italic">
        <h1 class="font-bold py-3 px-2 text-lg">Gallery</h1>
      </div>
      <div class="grid grid-cols-1 gap-3 sm:grid-cols-3 md:grid-cols-3 lg:grid-cols-5 m-3">
        <div class="rounded-md text-center h-64 transition duration-200 transform hover:scale-105" :style="{'background-image':'url(https://upload.wikimedia.org/wikipedia/commons/6/6f/Earth_Eastern_Hemisphere.jpg)', 'background-position':'center', 'background-size':'cover'}"></div>
        <div class="rounded-md text-center h-64 transition duration-200 transform hover:scale-105" :style="{'background-image':'url('+require('@/assets/RickyCaesarAprillaTiaka.jpg')+')', 'background-position':'center', 'background-size':'cover'}"></div>
        <div class="rounded-md text-center h-64 transition duration-200 transform hover:scale-105" :style="{'background-image':'url('+require('@/assets/RickyCaesarAprillaTiaka.jpg')+')', 'background-position':'center', 'background-size':'cover'}"></div>
        <div class="rounded-md text-center h-64 transition duration-200 transform hover:scale-105" :style="{'background-image':'url('+require('@/assets/RickyCaesarAprillaTiaka.jpg')+')', 'background-position':'center', 'background-size':'cover'}"></div>
        <div class="rounded-md text-center h-64 transition duration-200 transform hover:scale-105" :style="{'background-image':'url('+require('@/assets/RickyCaesarAprillaTiaka.jpg')+')', 'background-position':'center', 'background-size':'cover'}"></div>
        <div class="rounded-md text-center h-64 transition duration-200 transform hover:scale-105" :style="{'background-image':'url('+require('@/assets/RickyCaesarAprillaTiaka.jpg')+')', 'background-position':'center', 'background-size':'cover'}"></div>
      </div>
      <!-- Github Contributions End -->
    </div>
    <Feeds/>
  </div>
  <!-- Container End -->
</template>
<script>
import Feeds from './view';
  export default {
    name: 'Profile',
    components : {
      Feeds
    },
    props: {
      msg: String,
      msg2: String,
    },
    variants: {
      extend: {
        boxSizing: false,
      }
    },
  }
</script>