<template>
  <transition name="fade" mode="out-in" appear>
    <div class="row row-body">
      <div class="hero">
        <div class="text-wrapper">
          <h1 class="">
            Project Rere supports Social Enterprises in Africa and Asia.
          </h1>
          <h3 class="upper bold mt-5">
            Season 1 of our Podcast is on the way!
          </h3>
          <h5 class="mt-2">
            Follow us to find our more about this season and our upcoming
            Request for Podcast.
          </h5>
          <div class="social-row">
            <a href="https://www.facebook.com/projectrere/" target="_blank">
              <b-img
                class="social-icons"
                :src="require('~/assets/images/icons/facebook-icon.svg')"
                alt="Facebook"
              ></b-img>
            </a>

            <a href="https://www.facebook.com/projectrere/" target="_blank">
              <b-img
                class="social-icons"
                :src="require('~/assets/images/icons/insta-icon.svg')"
                alt="Instagram"
              ></b-img>
            </a>
          </div>
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
          <div class="winners-container info">
            <h2 class="">
              Welcome and Congratulations to Project Rere Season 1 Winners!
            </h2>
            <div class="winners-cards-container pb-5">
              <div class="row agroCenter">
                <div class="col agroData team-card">
                  <b-img
                    :src="require('~/assets/images/winners/AgroData.png')"
                    alt=""
                    rounded="circle"
                  ></b-img>
                  <h3 class="team-name">AGRO DATA</h3>
                  <p class="team-bio">
                    Agro Data deploys a bee-centered cropping model, using honey
                    bees as pollinators for fruits and vegetable farming...
                  </p>
                  <!-- Button trigger modal -->
                  <button
                    v-b-modal="'argodata-bio'"
                    class="button button-no-border"
                  >
                    Learn More
                  </button>

                  <!-- Agro Data modal -->
                  <b-modal id="argodata-bio" hide-footer="true">
                    <div class="team-card">
                      <b-img
                        :src="require('~/assets/images/winners/agrodata-2.png')"
                        alt=""
                        rounded="circle"
                      ></b-img>
                      <h3 class="team-name">AGRO DATA</h3>
                      <div class="bios">
                        <p class="bio">
                          AgroData® deploys a bee-centred cropping model using
                          honey bees as pollinators for fruits and vegetable
                          farming. We enlist smallholder crop farmers into a
                          Community Bee AgriFood Network (CoBAN) and installs
                          beehives (for free) on their farmlands in a
                          partnership deal. We aggregate RAW HONEY across these
                          farms and package as FRESHDEW HONEY (NAFDAC
                          Certified); sharing the revenue with the smallholder
                          farmers.
                        </p>
                        <p class="bio">
                          We use innovative tech with sustainable practices to
                          improve farm productivity and rural livelihoods. We
                          enhance the bees-crops interaction with the invention
                          of the iSmart Hive (an IoT device) and we provide
                          Pollination as a Service. AgroData iSmarthive®
                          promotes rapid bee’s colonization towards pollination
                          of crops, enhances raw honey collection and collates
                          agro-ecological data from the environment, which helps
                          in the management of the Bees_Crops ecosystem.
                        </p>
                        <br />
                        <p class="bio"></p>
                      </div>
                    </div>
                  </b-modal>
                </div>
              </div>
              <div class="row">
                <div class="col team-card">
                  <b-img
                    :src="require('~/assets/images/winners/PetsPoint.png')"
                    alt=""
                    rounded="circle"
                  ></b-img>
                  <h3 class="team-name">PETSPOINT RECYLING</h3>
                  <p class="team-bio">
                    PETsPoint is an integrated clean tech value chain social
                    enterprise, we are leveraging technology to deploy mobile
                    application that allows aggregation of...
                  </p>
                  <!-- Button trigger modal -->
                  <button
                    v-b-modal="'petspoint-bio'"
                    class="button button-no-border"
                  >
                    Learn More
                  </button>

                  <!-- Agro Data modal -->
                  <b-modal id="petspoint-bio" hide-footer="true">
                    <div class="team-card">
                      <b-img
                        :src="require('~/assets/images/winners/PetsPoint.png')"
                        alt=""
                        rounded="circle"
                      ></b-img>
                      <h3 class="team-name">PETsPoint Recyling</h3>
                      <div class="bios">
                        <p class="bio">
                          PETsPoint is an integrated clean tech value chain
                          social enterprise, we are leveraging technology to
                          deploy mobile application that allows aggregation of
                          plastic waste directly from households, communities,
                          market place, event centres, including public and
                          private facilities through provision of community
                          collection infrastructures “receptacles” while using
                          incentives to drive desired behaviours and empower
                          semi-skilled women and girls from low income
                          communities. The recovered recyclables will be
                          recycled to manufacture high quality eco-friendly
                          products starting with bricks for the building
                          industry in short term with a long term plan and
                          expansion to production of yarns/fibres, t-shirts and
                          other consumables in the value chain.
                        </p>
                        <br />
                        <p class="bio">
                          Our mobile/digital platform “Junkyard” allows citizens
                          dispose their recyclable waste through a seamless
                          technological process and earn incentives. It also
                          allows waste management companies who register as a
                          collector on the app to collect recyclable waste
                          products through a seamless process. It comes with an
                          administrative panel which is the data collection web
                          app of the solution.
                        </p>
                      </div>
                    </div>
                  </b-modal>
                </div>
                <div class="col team-card">
                  <b-img
                    :src="require('~/assets/images/winners/recyclegh.png')"
                    alt=""
                    rounded="circle"
                  ></b-img>
                  <h3 class="team-name">RECYCLEGARB</h3>
                  <p class="team-bio">
                    ReceycleGarb operate a waste recycling scheme that motivates
                    and benefits grass root communities and informal waste
                    pickers...
                  </p>
                  <!-- Button trigger modal -->
                  <button
                    v-b-modal="'recyclegh-bio'"
                    class="button button-no-border"
                  >
                    Learn More
                  </button>

                  <!-- Agro Data modal -->
                  <b-modal id="recyclegh-bio" hide-footer="true">
                    <div class="team-card">
                      <b-img
                        :src="require('~/assets/images/winners/recyclegh.png')"
                        alt=""
                        rounded="circle"
                      ></b-img>
                      <h3 class="team-name">RecylceGarb</h3>
                      <div class="bios">
                        <p class="bio">
                          We operate a waste recycling scheme that motivates and
                          benefits grass root communities and informal waste
                          pickers. We are a social enterprise whose mission is
                          to create income and development opportunities for
                          individuals and communities by tackling poverty,
                          hunger, menstrual poverty and access to education
                          through waste recovery and recycling across Nigeria
                          and Africa.
                        </p>
                        <br />
                        <p class="bio">
                          The grant fund will enable us scale up our waste
                          recovering operations, thereby providing more income
                          opportunities for underprivileged low income
                          communities. The grant will also enable us implement
                          our Green Bank project, where low income communities
                          have access to foodstuffs, pay their children's school
                          fee ,as well as being able to afford monthly sanitary
                          pads monthly.
                        </p>
                      </div>
                    </div>
                  </b-modal>
                </div>
              </div>
            </div>
          </div>
          <div class="divider"></div>
          <div class="info pt-5">
            <h2 class="">
              We hope to inspire more people to support Social Enterprises, and
              begin their own social impact journey.
            </h2>
            <div class="info-cards-container row">
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
          <div class="divider"></div>
          <div class="join">
            <h2>
              Join us as we promote positive social change across Africa and
              Asia
            </h2>
            <iframe
              id="JotFormIFrame-90142788412154"
              allowtransparency="true"
              title="Trainee Registration Form"
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
              @load="iframeStyles"
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
import $ from 'jquery'
export default {
  transition: {
    name: 'home',
    mode: 'out-in',
  },
  mounted() {
    this.$nextTick(() => {
      this.$nuxt.$loading.start()

      setTimeout(() => {
        // const iframe = document.getElementById('JotFormIFrame-90142788412154')
        // $('iframe').contents().find('.formFooter').css('display', 'none')
        const frame = $('iframe').get(0)
        console.log(
          'check loading ',
          $(frame.body)
          // iframe.contentWindow // TODOs get the formfooter children
        )
        this.$nuxt.$loading.finish()
      }, 500)
    })
  },
  methods: {
    iframeStyles() {
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

<style scoped>
.home-enter-active,
.home-leave-active {
  transition: opacity 0.75s;
}
.home-enter,
.home-leave-active {
  opacity: 0;
}
.fade-enter-active,
.fade-leave-active {
  transition: opacity 0.25s ease-out;
}

.fade-enter,
.fade-leave-to {
  opacity: 0;
}

.team-name {
  font-size: 20px;
  margin: 5px 0;
  color: #4d4d4d;
}

.team-bio {
  font-size: 16px;
  color: #4d4d4d;
}

.text-wrapper {
  max-width: 576px;
}

.divider {
  width: 90%;
  border: 1px solid #01d6fa;
}

@media (min-width: 1200px) {
  .text-wrapper {
    max-width: 700px;
  }
}

@media (min-width: 1400px) {
  .text-wrapper {
    max-width: 900px;
  }
}
</style>
