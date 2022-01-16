<template>
  <div id="app">
    <div id="home">
      <Hero />
    </div>
    <div class="koala__main-content">
      <div id="introduce">
        <Introduce />
      </div>
      <div id="faq">
        <FAQ />
      </div>
      <div id="roadmap">
        <Roadmap />
      </div>
      <div id="minting">
        <Mint />
      </div>
    </div>
  </div>
</template>

<script>
import Hero from '~/components/Hero/Hero.vue'
import Introduce from '~/components/Introduce/Introduce.vue'
import FAQ from '~/components/FAQ/FAQ.vue'
import Roadmap from '~/components/Roadmap/Roadmap.vue'
import Mint from '~/components/Mint/Mint.vue'
export default {
  name: 'IndexPage',
  components: {
    Hero,
    Introduce,
    FAQ,
    Roadmap,
    Mint,
  },
}
</script>
