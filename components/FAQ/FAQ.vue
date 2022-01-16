<template>
  <div class="h-screen relative bg-gradient-to-br from-cyan-500 to-purple-900">
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
    <div
      class="absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2"
    >
      <div class="koala__faq-button">
        <button
          class="my-3 bg-cyan-400 w-full p-5 rounded-[20px] text-[30px] shadow-md shadow-slate-800 text-white hover:bg-cyan-500 active:bg-cyan-500 md:text-[27px]"
          @click="handleAnswerOne()"
        >
          what is the lazy koala club nft ?
        </button>
        <transition name="home">
          <button
            v-show="showAnswerOne"
            class="transform my-3 bg-white w-full p-5 rounded-[20px] text-[30px] shadow-md shadow-slate-800 text-cyan-400 md:text-[27px]"
          >
            what is the lazy koala club nft ?
          </button>
        </transition>
        <!--  -->
        <button
          class="my-3 bg-cyan-400 w-full p-5 rounded-[20px] text-[30px] shadow-md shadow-slate-800 text-white hover:bg-cyan-500 active:bg-cyan-500 md:text-[27px]"
          @click="handleAnswerTwo()"
        >
          when is the mint ?
        </button>
        <transition name="home">
          <button
            v-show="showAnswerTwo"
            class="transform my-3 bg-white w-full p-5 rounded-[20px] text-[30px] shadow-md shadow-slate-800 text-cyan-400 md:text-[27px]"
          >
            when is the mint?
          </button>
        </transition>
        <!--  -->
        <button
          class="my-3 bg-cyan-400 w-full p-5 rounded-[20px] text-[30px] shadow-md shadow-slate-800 text-white hover:bg-cyan-500 active:bg-cyan-500 md:text-[27px]"
          @click="handleAnswerThree()"
        >
          what is the total supply ?
        </button>
        <transition name="home">
          <button
            v-show="showAnswerThree"
            class="transform my-3 bg-white w-full p-5 rounded-[20px] text-[30px] shadow-md shadow-slate-800 text-cyan-400 md:text-[27px]"
          >
            what is the total supply ?
          </button>
        </transition>
        <!--  -->
        <button
          class="my-3 bg-cyan-400 p-5 w-full rounded-[20px] text-[30px] shadow-md shadow-slate-800 text-white md:text-[27px] hover:bg-cyan-500 active:bg-cyan-500"
          @click="handleAnswerFour()"
        >
          project goals ?
        </button>
        <transition name="home">
          <button
            v-show="showAnswerFour"
            class="transform my-3 bg-white w-full p-5 rounded-[20px] text-[30px] shadow-md shadow-slate-800 text-cyan-400 md:text-[27px]"
          >
            what is the total supply ?
          </button>
        </transition>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'RoadmapComponent',
  data() {
    return {
      showAnswerOne: false,
      showAnswerTwo: false,
      showAnswerThree: false,
      showAnswerFour: false,
    }
  },
  methods: {
    handleAnswerOne() {
      this.showAnswerOne = !this.showAnswerOne
      this.showAnswerTwo = false
      this.showAnswerThree = false
      this.showAnswerFour = false
    },
    handleAnswerTwo() {
      this.showAnswerTwo = !this.showAnswerTwo
      this.showAnswerOne = false
      this.showAnswerThree = false
      this.showAnswerFour = false
    },
    handleAnswerThree() {
      this.showAnswerThree = !this.showAnswerThree
      this.showAnswerOne = false
      this.showAnswerTwo = false
      this.showAnswerFour = false
    },
    handleAnswerFour() {
      this.showAnswerFour = !this.showAnswerFour
      this.showAnswerOne = false
      this.showAnswerTwo = false
      this.showAnswerThree = false
    },
  },
}
</script>
<style scoped>
.home-enter-active,
.home-leave-active {
  transition: opacity 0.5s ease-in-out;
}
.home-enter,
.home-leave-active {
  opacity: 0;
}
</style>
