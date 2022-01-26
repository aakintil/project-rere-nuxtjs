<template>
  <div class="row row-header">
    <b-navbar
      toggleable="lg"
      type="light"
      color="light"
      variant="light"
      fixed="top"
    >
      <b-navbar-brand target="nav-collapse">
        <!-- <nuxt-link to="/" v-model="showCollapse"> -->
        <!-- TODOs
        see if we can get the navbar to collapse when you tap the logo -->
        <Logo />
        <!-- </nuxt-link> -->
      </b-navbar-brand>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">
          <b-nav-item to="/" class="button-links mg-right"> Home </b-nav-item>
          <b-nav-item to="/about" class="button-links"> About </b-nav-item>
          <!-- <b-nav-item
            to="/apply"
            class="button button-sm button-outline-primary button-links"
          >
            Apply
          </b-nav-item> -->
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>
