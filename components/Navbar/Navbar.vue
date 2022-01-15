<template>
  <div :class="{ scrolled: isScroll }" class="sticky top-0 z-50 koala__navbar">
    <div class="absolute z-10 w-full flex justify-between items-center p-10">
      <div class="koala__navbar-left-content">
        <nuxt-link
          :to="{ path: '/', hash: 'home' }"
          class="koala__navbar-text px-5 py-3 lg:text-[36px]"
        >
          Home
        </nuxt-link>
      </div>
      <div class="koala__navbar-right-content flex">
        <nuxt-link
          :to="{ path: '/', hash: 'introduce' }"
          class="koala__navbar-text px-5 py-3 lg:text-[36px]"
        >
          Inroduce
        </nuxt-link>
        <nuxt-link
          :to="{ path: '/', hash: 'faq' }"
          class="koala__navbar-text px-5 py-3 lg:text-[36px]"
        >
          FAQ
        </nuxt-link>
        <nuxt-link
          :to="{ path: '/', hash: 'roadmap' }"
          class="koala__navbar-text px-5 py-3 lg:text-[36px]"
        >
          roadmap
        </nuxt-link>
        <nuxt-link
          :to="{ path: '/', hash: 'mint' }"
          class="koala__navbar-text px-5 py-3 lg:text-[36px]"
        >
          mint
        </nuxt-link>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'KoalaNavbar',
  data() {
    return {
      isScroll: false,
    }
  },
  beforeMount() {
    window.addEventListener('scroll', this.handleScroll)
  },
  beforeDestroy() {
    window.removeEventListener('scroll', this.handleScroll)
  },
  methods: {
    handleScroll() {
      // Your scroll handling here
      console.log(window.scrollY)
      if (window.scrollY > 0) {
        this.isScroll = true
      } else {
        this.isScroll = false
      }
    },
  },
}
</script>
<style lang="scss">
.scrolled {
  height: 9rem;
  background: rgb(2, 0, 36);
  background: linear-gradient(
    120deg,
    rgba(2, 0, 36, 1) 0%,
    rgba(0, 212, 255, 1) 0%,
    rgba(51, 13, 105, 1) 100%
  );
}
</style>
