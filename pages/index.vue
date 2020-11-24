<template>
  <div class="row row-body">
    <div class="hero">
      <div class="text-wrapper">
        <h1 class="title">
          Project Rere supports Social Enterprises in Africa and Asia.
        </h1>
        <h5 class="mt-5">
          Working on improving access to Education in Nigeria? Apply now for our
          Podcast and Grant!
        </h5>
        <nuxt-link to="/apply" class="button button-primary button-lg mt-2">
          Apply
        </nuxt-link>
      </div>
      <div class="overlay"></div>
      <b-img
        fluid
        class="hero-image"
        :src="require('~/assets/images/hero-banner.jpg')"
        alt="Responsive image"
      ></b-img>
    </div>
    <div class="content"></div>
  </div>
</template>

<script>
export default {}
</script>

<style></style>
