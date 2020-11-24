<template>
  <div :class="checkRoutes" class="row row-footer">
    <div class="footer">
      <nuxt-link v-if="checkRoutes === 'home'" to="/" class="navbar-brand">
        <img
          class="header-logo"
          loading="auto"
          src="~/assets/images/logos/projectrere-logo-white.svg"
          alt=""
        />
      </nuxt-link>
      <a
        href="https://docs.google.com/document/d/1WcHhkeq4FBVVHUXvXnpjsHdPm4fkvGhRWTL6sWCLKzI/edit?usp=sharing"
        target="_blank"
        class="text-links"
        >Privacy Policy</a
      >
      <a href="mailto:hello@projectrere.com" target="_blank" class="text-links">
        Contact us at hello@projectrere.com
      </a>
      <p class="caption">Copyright &#169; Project Rere Ltd</p>
    </div>
  </div>
</template>
<script>
export default {
  computed: {
    checkRoutes() {
      if (this.$route.path === '/about') return 'about'
      if (this.$route.path === '/apply') return 'apply'
      return 'home'
    },
  },
}
</script>
