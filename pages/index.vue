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
          <h1 class="">
            Project Rere supports Social Enterprises in Africa and Asia.
          </h1>
          <h5 class="mt-5">
            Working on improving access to Education in Nigeria? Apply now for
            our Podcast and Grant!
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
      <div class="content">
        <div class="content-wrapper">
          <div class="info">
            <h2 class="">
              We hope to inspire more people to support Social Enterprises, and
              begin their own social impact journey.
            </h2>
            <div class="info-cards-container">
              <div class="info-card">
                <b-img
                  class="info-cards-img"
                  :src="require('~/assets/images/icons/awareness-icon.png')"
                  alt="Responsive image"
                ></b-img>
                <h3>Awareness</h3>
                <p class="caption">
                  We share stories about and provide grants to Social
                  Enterprises in Africa and Asia.
                </p>
              </div>
              <div class="info-card">
                <b-img
                  class="info-cards-img"
                  :src="require('~/assets/images/icons/podcasts-icon.png')"
                  alt="Responsive image"
                ></b-img>
                <h3>Podcasts</h3>
                <p class="caption">
                  Through stories, we aim to provide Social Enterprises access
                  to an audience of curious listeners and investors.
                </p>
              </div>
              <div class="info-card">
                <b-img
                  class="info-cards-img"
                  :src="require('~/assets/images/icons/grants-icon.png')"
                  alt="Responsive image"
                ></b-img>
                <h3>Grants</h3>
                <p class="caption">
                  We use our grant capital to support the growth of creative and
                  innovative ideas developed by Social Entrepreneurs.
                </p>
              </div>
            </div>
          </div>
          <div class="join">
            <h2>
              Join us as we promote positive social change across Africa and
              Asia
            </h2>
            <iframe
              META
              HTTP-EQUIV="Access-Control-Allow-Origin"
              id="JotFormIFrame-90142788412154"
              title="Trainee Registration Form"
              @load="iframeStyles"
              allowtransparency="true"
              allowfullscreen="true"
              allow="geolocation; microphone; camera"
              src="https://form.jotform.com/202654195519056"
              frameborder="0"
              style="
                width: 1px;
                min-width: 100%;
                min-height: 500px;
                height: 100%;
                border: none;
              "
              scrolling="yes"
            ></iframe>
          </div>
        </div>
      </div>
      <div class="footer">
        <b-img
          class="header-logo"
          loading="auto"
          :src="require('~/assets/images/logos/projectrere-logo-white.svg')"
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
  mounted() {
    this.$nextTick(() => {
      this.$nuxt.$loading.start()

      setTimeout(() => {
        const iframe = document.getElementById('JotFormIFrame-90142788412154')

        console.log(
          'check loading ',
          $
          // iframe.contentWindow // TODOs get the formfooter children
        )
        this.$nuxt.$loading.finish()
      }, 4500)
    })
  },
  methods: {
    iframeStyles() {
      console.log(
        'calling iframe styles ---------------- ',
        this.$refs.contentWindow
      )
      // this.frame = this.$refs.iframeContent.contentWindow

      // const style =
      //   '.layout__wrapper {background:' +
      //   this.background +
      //   ';} ' +
      //   'body {color:' +
      //   this.text +
      //   ';} '
      // this.frame.postMessage(style, '*')
    },
  },
}
</script>

<style>
.home-enter-active,
.home-leave-active {
  transition: opacity 0.75s;
}
.home-enter,
.home-leave-active {
  opacity: 0;
}
</style>
