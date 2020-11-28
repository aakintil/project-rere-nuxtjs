<template>
  <div class="container-fluid">
    <Header />
    <Nuxt />
  </div>
</template>

<script>
import $ from 'jquery'
import Header from '~/components/Header.vue'

export default {
  components: {
    Header,
  },
  mounted() {
    $('.container-fluid').fadeTo(750, 1)
  },
}
</script>
