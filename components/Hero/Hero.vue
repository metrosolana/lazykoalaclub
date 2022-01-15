<template>
  <div id="home" class="koala__hero-component">
    <div
      class="relative h-screen w-full bg-gradient-to-br from-cyan-500 to-purple-900"
    >
      <div
        class="absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 drop-shadow-2xl lg:h-80 lg:w-80 md:h-72 md:w-72 sm:h-60 sm:w-60 rounded-full bg-gradient-to-br from-cyan-500 to-purple-900"
      ></div>
      <div
        class="absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2"
      >
        <h1
          class="text-white uppercase koala__hero-header-text lg:text-[72px] md:text-[42px] sm:text-[35px]"
        >
          lazy koala club
        </h1>
        <p
          class="text-center text-white uppercase koala__hero-description-text lg:text-[24px] md:text-[23px] sm:text-[18px]"
        >
          everyday is sleep
        </p>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'HeroComponent',
}
</script>
