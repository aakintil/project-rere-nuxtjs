<template>
  <div class="container-fluid">
    <Header />
    <Nuxt />
  </div>
</template>

<script>
import Header from '~/components/Header.vue'

export default {
  components: {
    Header,
  },
}
</script>
