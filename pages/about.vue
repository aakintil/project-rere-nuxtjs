<template>
  <transition
    name="home"
    mode="in-out"
    appear
    appear-class="custom-appear-class"
  >
    <div class="row row-body">
      <div class="hero">
        <div class="text-wrapper">
          <h1 class="">Rere (ray-ray) in Yoruba means positive, positivity.</h1>
          <h5 class="mt-5">
            Project Rere shares stories about Social Entrepreneurs who are
            making a difference, particularly in Africa and Asia. Our team aims
            to shine a light on the positive impact being created by Social
            Enterpreneurs across global communities.
          </h5>
        </div>
        <div class="overlay"></div>
        <b-img
          fluid
          class="hero-image"
          :src="require('~/assets/images/about-banner.jpg')"
          alt="Responsive image"
        ></b-img>
      </div>
      <div class="content">
        <div class="content-wrapper">
          <h2 class="">
            We are all passionate people, committed to making the world a better
            place. Read more about us below!
          </h2>

          <h2 class="team-section-titles">Our Team</h2>
          <div class="team">
            <div class="team-card vivek">
              <b-img
                :src="require('~/assets/images/team/vivek.png')"
                alt=""
              ></b-img>
              <h3 class="team-name">Vivek Aswani</h3>
              <p class="team-role">The Finance Ninja</p>
              <!-- Button trigger modal -->
              <b-button v-b-modal="'vivek-bio'">Learn More</b-button>

              <!-- Viveks modal -->
              <b-modal id="vivek-bio">
                <div class="team-card">
                  <b-img
                    :src="require('~/assets/images/team/vivek.png')"
                    alt=""
                  ></b-img>
                  <h3 class="team-name">Vivek Aswani</h3>
                  <p class="team-role">The Finance Ninja</p>
                  <div class="bios">
                    <p class="bio">
                      A 4th Generation Tolaram Group Family member, Singaporean
                      born but Nigeria raised. He is a serial entrepreneur
                      having started his career in the F&B industry and most
                      recently opened a cocktail bar in Singapore called The
                      Barbary Coast. Vivek currently works in Nigeria as part of
                      the Tolaram Group Beverage division having developed a
                      brand called GoodLife Magik which is a fruit drink aimed
                      at the children in Nigeria.
                    </p>
                    <br />
                    <p class="bio">
                      Having made investments in many companies, Vivek realised
                      that access to finance was needed for Social Entrepreneurs
                      to scale their impact. Project Rere was created to
                      showcase Social Enterprises, busy with saving the world,
                      and to provide them with access to potential grants and
                      investments. Vivek has a MA in Economics and Finance and
                      in his free time loves to go diving and drinking single
                      malt whiskey.
                    </p>
                  </div>
                </div>
              </b-modal>
            </div>
          </div>
        </div>
      </div>
      <div class="footer">
        <b-img
          class="header-logo"
          loading="auto"
          :src="require('~/assets/images/logos/projectrere-logo-black.svg')"
          alt=""
        />
        <a
          href="https://docs.google.com/document/d/1WcHhkeq4FBVVHUXvXnpjsHdPm4fkvGhRWTL6sWCLKzI/edit?usp=sharing"
          target="_blank"
          class="text-links"
          >Privacy Policy</a
        >
        <a
          href="mailto:hello@projectrere.com"
          target="_blank"
          class="text-links"
        >
          Contact us at hello@projectrere.com
        </a>
        <p class="caption">Copyright &#169; Project Rere Ltd</p>
      </div>
    </div>
  </transition>
</template>

<script>
export default {
  transition: {
    name: 'home',
    mode: 'out-in',
  },
  mounted() {},
  methods: {},
}
</script>

<style scoped>
.home-enter-active,
.home-leave-active {
  transition: opacity 0.75s;
}
.home-enter,
.home-leave-active {
  opacity: 0;
}

.hero-image {
  max-width: 300%;
}

.content,
.footer {
  background: #f5f13e;
}

.footer .text-links,
.footer p {
  color: black;
}

@media (min-width: 992px) {
  .hero-image {
    max-width: 150%;
  }
}

@media (min-width: 1200px) {
  .hero-image {
    max-width: 100%;
  }
  .text-wrapper h1 {
    max-width: 1100px;
  }
  .text-wrapper h5 {
    max-width: none;
  }
}
</style>
