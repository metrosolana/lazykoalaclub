<template>
  <div class="relative h-screen bg-gradient-to-br from-cyan-500 to-purple-900">
    <div
      class="absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 drop-shadow-2xl lg:h-80 lg:w-80 md:h-72 md:w-72 sm:h-60 sm:w-60 rounded-full bg-gradient-to-br from-cyan-500 to-purple-900"
    ></div>
    <div
      class="absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 opacity-10"
    >
      <h1
        class="text-white uppercase koala__hero-header-text text-[72px] md:text-[45px] sm:text-[35px]"
      >
        lazy koala club
      </h1>
      <p
        class="text-center text-white uppercase koala__hero-description-text lg:text-[24px] md:text-[23px] sm:text-[18px]"
      >
        everyday is sleep
      </p>
    </div>
    <div class="koala__roadmap">
      <h1
        class="text-white text-[72px] md:text-[50px] absolute top-[40%] left-1/2 transform -translate-x-1/2 -translate-y-1/2"
      >
        Roadmap
      </h1>
      <div
        class="koala__roadmap-phase-dot flex items-center absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 w-full mt-16"
      >
        <img src="~/assets/img/roadmap-graphic.png" alt="" />
      </div>
    </div>
    <div
      class="koala__roadmap-text absolute top-1/2 left-1/4 transform -translate-x-24 translate-y-20"
    >
      <div>
        <p class="text-cyan-400 text-[30px]">phase 1</p>
        <ul>
          <li class="text-cyan-400">minting</li>
          <li class="text-cyan-400">listing</li>
        </ul>
      </div>
    </div>
    <!--  -->
    <div
      class="koala__roadmap-text absolute top-1/2 left-1/4 transform translate-x-32 -translate-y-16"
    >
      <div>
        <p class="text-white text-[30px]">phase 2</p>
        <ul>
          <li class="text-white">drd verification</li>
          <li class="text-white">rarity</li>
        </ul>
      </div>
    </div>
    <!--  -->
    <div
      class="koala__roadmap-text absolute top-1/2 right-1/4 transform -translate-x-20 translate-y-20"
    >
      <div>
        <p class="text-white text-[30px]">phase 3</p>
        <ul>
          <li class="text-white">donate</li>
        </ul>
      </div>
    </div>
    <!--  -->
    <div
      class="koala__roadmap-text absolute top-1/2 right-1/4 transform translate-x-52 -translate-y-16"
    >
      <div>
        <p class="text-white text-[30px]">phase 4</p>
        <ul>
          <li class="text-white">realised roadmap 2.0</li>
        </ul>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'RoadmapComponent',
}
</script>
<style scoped>
.koala__roadmap-text ul li:before {
  content: '- ';
}
</style>
