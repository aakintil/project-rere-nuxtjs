<template>
  <div>
    <b-navbar toggleable="lg" type="light" color="light" variant="light">
      <b-navbar-brand>
        <nuxt-link to="/">
          <Logo />
        </nuxt-link>
      </b-navbar-brand>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">
          <nuxt-link to="/"> Home </nuxt-link>
          <nuxt-link to="/about"> About </nuxt-link>
          <nuxt-link to="/apply"> Apply </nuxt-link>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>
