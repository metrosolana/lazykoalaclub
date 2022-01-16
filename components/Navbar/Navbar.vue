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
          Introduce
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
          :to="{ path: '/', hash: 'minting' }"
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
      if (window.scrollY > 0) {
        this.isScroll = true
      } else {
        this.isScroll = false
      }
    },
  },
}
</script>
