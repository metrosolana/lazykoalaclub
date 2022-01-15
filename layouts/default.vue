<template>
  <div>
    <Navbar />
    <Nuxt />
  </div>
</template>
<script>
import Navbar from '~/components/Navbar/Navbar.vue'
export default {
  name: 'DefaultLayout',
  components: {
    Navbar,
  },
}
</script>
