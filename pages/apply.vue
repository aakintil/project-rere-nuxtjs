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
            Dear Changemakers, Project Rere would like to share your story!
          </h1>
          <h5 class="mt-5">
            2020 has been a difficult year for so many and we would like to help
            in the best way we can, by sharing stories about the great work
            being done by Social Entrepreneurs on the ground, and helping to
            fund their Social Enterprises.
          </h5>
          <h5>
            Apply now for our Podcast! Successful applicants will get a chance
            to share their story with the world and receieve grant funding of up
            to US $25,000.
          </h5>
        </div>
        <div class="overlay"></div>
        <b-img
          fluid
          class="hero-image"
          :src="require('~/assets/images/apply-banner.jpg')"
          alt=""
        ></b-img>
      </div>
      <div class="content">
        <div class="content-wrapper">
          <div class="info">
            <b-tabs content-class="mt-3" align="center">
              <b-tab title="Apply" active>
                <h2 class="mt-5 mb-2">Apply</h2>
                <div class="apply-wrapper">
                  <p>
                    For the first round of our podcasts, we are going to
                    showcase 4-6 outstanding social enterprises which focus on
                    Education in Nigeria. If you’re doing great work in another
                    sector or region, look out for our future RFPs (Request For
                    Podcasts), and View our season schedule above.
                  </p>
                  <br />
                  <p>
                    Simply fill out the form below to submit your application.
                    Applications for Season 1 of the RFP closes on (specify
                    date) and we will announce the successful applicants 4 weeks
                    later. Each applicant that qualifies will receive the chance
                    to share their story to the world and receive up to
                    <span class="bold"> US $25,000 </span> in grant funding.
                  </p>
                  <br />
                  <span class="underline"> Criteria </span>
                  <ol type="1">
                    <li>Solving a social problem based on our season</li>
                    <li>A Social Business that displays the following:</li>
                    <ol type="a">
                      <li>Social Impact</li>
                      <li>Financial Returns</li>
                      <li>
                        The social element is built in the business model. You
                        involve the community and those who are vulnerable or in
                        need in your enterprise. You are empowering them to do
                        better - not just teaching them to fish, but also
                        bringing them to the market.
                      </li>
                    </ol>
                  </ol>
                  <div class="title-row">
                    <h3 class="small-mg-btm mt-5 mb-4">Application Form</h3>
                  </div>
                  <iframe
                    id="JotFormIFrame-90142788412154"
                    allowtransparency="true"
                    title="Trainee Registration Form"
                    allowfullscreen="true"
                    allow="geolocation; microphone; camera"
                    src="https://form.jotform.com/202644218197053"
                    frameborder="0"
                    style="
                      width: 1px;
                      min-width: 100%;
                      min-height: 1480px;
                      height: 100%;
                      border: none;
                    "
                    scrolling="yes"
                  ></iframe>
                </div>
              </b-tab>
              <b-tab title="FAQs">
                <h2 class="mt-5 mb-2">FAQs</h2>
                <div class="accordion" role="tablist">
                  <b-card no-body class="mb-1">
                    <b-card-header header-tag="header" class="p-1" role="tab">
                      <b-button v-b-toggle.accordion-1 block variant="info"
                        >How long is a season?
                      </b-button>
                    </b-card-header>
                    <b-collapse
                      id="accordion-1"
                      visible
                      accordion="my-accordion"
                      role="tabpanel"
                    >
                      <b-card-body>
                        <b-card-text>{{ season }}</b-card-text>
                      </b-card-body>
                    </b-collapse>
                  </b-card>

                  <b-card no-body class="mb-1">
                    <b-card-header header-tag="header" class="p-1" role="tab">
                      <b-button v-b-toggle.accordion-2 block variant="info"
                        >How long in the assessment period for each
                        RFP?</b-button
                      >
                    </b-card-header>
                    <b-collapse
                      id="accordion-2"
                      accordion="my-accordion"
                      role="tabpanel"
                    >
                      <b-card-body>
                        <b-card-text>{{ assessment }}</b-card-text>
                      </b-card-body>
                    </b-collapse>
                  </b-card>

                  <b-card no-body class="mb-1">
                    <b-card-header header-tag="header" class="p-1" role="tab">
                      <b-button v-b-toggle.accordion-3 block variant="info"
                        >Once my application is approved, what next?
                      </b-button>
                    </b-card-header>
                    <b-collapse
                      id="accordion-3"
                      accordion="my-accordion"
                      role="tabpanel"
                    >
                      <b-card-body>
                        <b-card-text>{{ approval }}</b-card-text>
                      </b-card-body>
                    </b-collapse>
                  </b-card>

                  <b-card no-body class="mb-1">
                    <b-card-header header-tag="header" class="p-1" role="tab">
                      <b-button v-b-toggle.accordion-4 block variant="info"
                        >What is the season lineup?
                      </b-button>
                    </b-card-header>
                    <b-collapse
                      id="accordion-4"
                      accordion="my-accordion"
                      role="tabpanel"
                    >
                      <b-card-body>
                        <b-card-text>{{ lineup }}</b-card-text>
                      </b-card-body>
                    </b-collapse>
                  </b-card>

                  <b-card no-body class="mb-1">
                    <b-card-header header-tag="header" class="p-1" role="tab">
                      <b-button v-b-toggle.accordion-5 block variant="info"
                        >Can I reapply for a future season?
                      </b-button>
                    </b-card-header>
                    <b-collapse
                      id="accordion-5"
                      accordion="my-accordion"
                      role="tabpanel"
                    >
                      <b-card-body>
                        <b-card-text>{{ reapply }}</b-card-text>
                      </b-card-body>
                    </b-collapse>
                  </b-card>

                  <b-card no-body class="mb-1">
                    <b-card-header header-tag="header" class="p-1" role="tab">
                      <b-button v-b-toggle.accordion-6 block variant="info"
                        >Why are some seasons country specific and others more
                        general?
                      </b-button>
                    </b-card-header>
                    <b-collapse
                      id="accordion-6"
                      accordion="my-accordion"
                      role="tabpanel"
                    >
                      <b-card-body>
                        <b-card-text>{{ specific }}</b-card-text>
                      </b-card-body>
                    </b-collapse>
                  </b-card>
                </div>
                <p class="faq-text">
                  If you have any other questions, please drop us an email at
                  <a href="mailto:hello@projectrere.com" target="_blank"
                    >hello@projectrere.com</a
                  >
                </p>
              </b-tab>
              <b-tab title="Schedule">
                <h2 class="mt-5 mb-2">Schedule</h2>
                <ol>
                  <li>Education in Nigeria - December 2020</li>
                  <li>Education in Indonesia - February 2021</li>
                  <li>Health Care - April 2021</li>
                  <li>Fintech - June 2021</li>
                  <li>Sanitation - August 2021</li>
                  <li>Climate Change - October 2021</li>
                </ol>
                <p class="faq-text">
                  Seasons are subject to change and this page will be updated
                  accordingly. Subscribe to our newsletter to stay informed.
                  Subsequent seasons will be added shortly.
                </p>
              </b-tab>
            </b-tabs>
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
  data() {
    return {
      season: `
Each season is between 4-6 episodes released over a month. The length of the season is dependent on the number of winning enterprises identified over the course of the RfP. Seasons are kept short to allow us to cover more countries, regions and social causes. 
        `,
      assessment: `Our team will assess all the applicants within 3 weeks of the closing date of the application period. All applicants will hear back on the status of their application 4 weeks after the closing date. `,
      approval: `Successful applicants will record a podcast episode with our team. The team will provide you with a list of the necessary software and other recording requirements. The team will require 2 sessions with you for the podcast. One to get to know you and your team, and the second to record the episode. `,
      lineup: `Our first season will cover Education in Nigeria. Subsequent seasons are listed on the Schedule Tab of the Apply page.`,
      reapply: `As long as your enterprise is relevant to the season, you are allowed to reapply. Winners of each season will not be permitted to reapply as we would like to cover as many deserving Social Enterprises as possible. `,
      specific: `The tentative schedule of our season is based on our current reach as well as feedback received on the potential Social Enterprises that fit a category. We are open to your feedback and suggestions on potential Social Enterprises, feel free to drop us an email at hello@projectrere.com`,
    }
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

.hero-image {
  max-width: 300%;
}

.content,
.footer {
  background: #03de98;
}

.apply-wrapper {
  text-align: left;
}

h2,
h3 {
  text-align: center;
}

.hero-image {
  margin-top: -520px;
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
  .text-wrapper {
    max-width: 700px;
  }
}

@media (min-width: 1400px) {
  .text-wrapper {
    max-width: 860px;
  }

  .text-wrapper h5 {
    max-width: none;
  }

  .hero {
    height: 128vh;
  }
}
</style>
