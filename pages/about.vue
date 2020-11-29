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
          alt=""
        ></b-img>
      </div>
      <div class="content">
        <div class="content-wrapper">
          <div class="info">
            <h2 class="">
              We are all passionate people, committed to making the world a
              better place. Read more about us below!
            </h2>

            <h3 class="team-section-titles mt-5">Our Team</h3>
            <div class="team">
              <!-- vivek -->
              <div class="team-card vivek">
                <b-img
                  :src="require('~/assets/images/team/vivek.png')"
                  alt=""
                ></b-img>
                <h3 class="team-name">Vivek Aswani</h3>
                <p class="team-role">The Finance Ninja</p>
                <!-- Button trigger modal -->
                <button class="button button-no-border" v-b-modal="'vivek-bio'">
                  Learn More
                </button>

                <!-- Viveks modal -->
                <b-modal hide-footer="true" id="vivek-bio">
                  <div class="team-card">
                    <b-img
                      :src="require('~/assets/images/team/vivek.png')"
                      alt=""
                    ></b-img>
                    <h3 class="team-name">Vivek Aswani</h3>
                    <p class="team-role">The Finance Ninja</p>
                    <div class="bios">
                      <p class="bio">
                        A 4th Generation Tolaram Group Family member,
                        Singaporean born but Nigeria raised. He is a serial
                        entrepreneur having started his career in the F&B
                        industry and most recently opened a cocktail bar in
                        Singapore called The Barbary Coast. Vivek currently
                        works in Nigeria as part of the Tolaram Group Beverage
                        division having developed a brand called GoodLife Magik
                        which is a fruit drink aimed at the children in Nigeria.
                      </p>
                      <br />
                      <p class="bio">
                        Having made investments in many companies, Vivek
                        realised that access to finance was needed for Social
                        Entrepreneurs to scale their impact. Project Rere was
                        created to showcase Social Enterprises, busy with saving
                        the world, and to provide them with access to potential
                        grants and investments. Vivek has a MA in Economics and
                        Finance and in his free time loves to go diving and
                        drinking single malt whiskey.
                      </p>
                    </div>
                  </div>
                </b-modal>
              </div>

              <!-- anusha -->
              <div class="team-card anusha">
                <b-img
                  :src="require('~/assets/images/team/anusha.png')"
                  alt=""
                ></b-img>
                <h3 class="team-name">Anusha Aswani</h3>
                <p class="team-role">The Social Impact Queen</p>
                <!-- Button trigger modal -->
                <button
                  class="button button-no-border"
                  v-b-modal="'anusha-bio'"
                >
                  Learn More
                </button>

                <!-- Viveks modal -->
                <b-modal hide-footer="true" id="anusha-bio">
                  <div class="team-card">
                    <b-img
                      :src="require('~/assets/images/team/anusha.png')"
                      alt=""
                    ></b-img>
                    <h3 class="team-name">Vivek Aswani</h3>
                    <p class="team-role">The Finance Ninja</p>
                    <div class="bios">
                      <p class="bio">
                        Her career first began in Corporate Communications and
                        soon made the switch to Philanthropy. Having initiated
                        various Social Projects in Nigeria, where she grew up,
                        she then decided to pursue her MBA in Social Impact.
                        Anusha has had 8 years in the Impact sphere and is
                        currently running a small Marketing and Distribution
                        company focusing on wholesome food and drink in
                        Singapore.
                      </p>
                      <br />
                      <p class="bio">
                        Not a Quant herself, Anusha has always believed that
                        finance would be able to make the world a better place,
                        and that’s what Project Rere aims to do. In her free
                        time, Anusha is usually found testing out a new recipe
                        or watching her football club, Arsenal, surprise her in
                        one way or another.
                      </p>
                    </div>
                  </div>
                </b-modal>
              </div>

              <!-- archibald -->
              <div class="team-card archibald">
                <b-img
                  :src="require('~/assets/images/team/archibald.png')"
                  alt=""
                ></b-img>
                <h3 class="team-name">Archibald Denis</h3>
                <p class="team-role">The Musical Maestro</p>
                <!-- Button trigger modal -->
                <button
                  class="button button-no-border"
                  v-b-modal="'archibald-bio'"
                >
                  Learn More
                </button>

                <!-- Archis modal -->
                <b-modal hide-footer="true" id="archibald-bio">
                  <div class="team-card">
                    <b-img
                      :src="require('~/assets/images/team/archibald.png')"
                      alt=""
                    ></b-img>
                    <h3 class="team-name">Archibald Denis</h3>
                    <p class="team-role">The Musical Maestro</p>
                    <div class="bios">
                      <p class="bio">
                        A French born world traveller. Having grown up in
                        Jakarta, Singapore and later the USA. Archibald is a
                        multi instrumentalist musician, at the age of 17 he was
                        accepted on scholarship to Berklee College of Music in
                        Boston MA where he attended Berklee for 4 years
                        graduating with his bachelors in Professional Music.
                      </p>
                      <br />
                      <p class="bio">
                        Archibald has been in numerous bands throughout the
                        years including; Bear Language, Figaro, Grey Area Trio
                        and today he is leading Superjava in his quest to
                        continue to spread his music to the world. Today he
                        writes and produces his music from his home studio
                        located near Bayonne, a town in the South West of
                        France.
                      </p>
                    </div>
                  </div>
                </b-modal>
              </div>

              <!-- aderinsola -->
              <div class="team-card aderinsola">
                <b-img
                  :src="require('~/assets/images/team/aderinsola.png')"
                  alt=""
                ></b-img>
                <h3 class="team-name">Aderinsola Akintilo</h3>
                <p class="team-role">The Tech Guru</p>
                <!-- Button trigger modal -->
                <button
                  class="button button-no-border"
                  v-b-modal="'aderinsola-bio'"
                >
                  Learn More
                </button>

                <!-- Archis modal -->
                <b-modal hide-footer="true" id="aderinsola-bio">
                  <div class="team-card">
                    <b-img
                      :src="require('~/assets/images/team/aderinsola.png')"
                      alt=""
                    ></b-img>
                    <h3 class="team-name">Aderinsola Akintilo</h3>
                    <p class="team-role">The Tech Guru</p>
                    <div class="bios">
                      <p class="bio">
                        Aderinsola Akintilo is a CEO, consultant, and designer
                        on a mission to build global alliances throughout
                        Nigeria and the African diaspora. He is currently a
                        co-founder of SiriusLabs, a software solutions company
                        specializing in mobile and web applications. He finds
                        himself moonlighting on music, finance, and agriculture
                        projects.
                      </p>
                      <br />
                      <p class="bio">
                        Aderinsola wants to make the world a better place, and
                        by working with ProjectRere he is able to by showing the
                        world that you can help people and make money at the
                        same time. In his free time, you can find Aderinsola
                        swimming in the ocean, playing football, and learning
                        how to build sustainable farms.
                      </p>
                    </div>
                  </div>
                </b-modal>
              </div>
            </div>
            <div class="advisor">
              <h3 class="team-section-titles mt-5">Our Advisor</h3>
              <div class="team-card nitin">
                <b-img
                  :src="require('~/assets/images/team/nitin.png')"
                  alt=""
                ></b-img>
                <h3 class="team-name">Nitin Vaswani</h3>
                <p class="team-role">The Social Finance Doctor</p>
                <!-- Button trigger modal -->
                <button class="button button-no-border" v-b-modal="'nitin-bio'">
                  Learn More
                </button>

                <!-- Archis modal -->
                <b-modal hide-footer="true" id="nitin-bio">
                  <div class="team-card">
                    <b-img
                      :src="require('~/assets/images/team/nitin.png')"
                      alt=""
                    ></b-img>
                    <h3 class="team-name">Nitin Vaswani</h3>
                    <p class="team-role">The Social Finance Doctor</p>
                    <div class="bios">
                      <p class="bio">
                        Nitin started his career at Oxley Capital Group, a
                        boutique private equity firm based in Singapore. He
                        advised clients on M&A transactions in the agriculture
                        and healthcare sectors across the Asia-Pacific region.
                        Nitin subsequently completed an MD at the University of
                        Queensland, and pursued specialty training in trauma
                        surgery. During his clinical training, he advised
                        philanthropic foundations on the deployment of safe and
                        cost-effective clinical protocols in their respective
                        healthcare centers. After his clinical training, Nitin
                        completed his MPH and MBA at Johns Hopkins University,
                        where he helped drive research on global surgical safety
                        issues.
                      </p>
                      <br />
                      <p class="bio">
                        More recently, he worked as an Investment Banking
                        Associate at J.P. Morgan’s Healthcare Group, and
                        co-founded a venture capital firm. Nitin was responsible
                        for launching the venture capital firm’s impact
                        investment arm, which advised a variety of family
                        offices on debt and equity transactions in the education
                        and healthcare sectors. Subsequently, Nitin worked in
                        the social investment and innovative financing group of
                        a global NGO named Pact, where he focused on sourcing
                        and completing investments linked to the organization’s
                        mission.
                      </p>
                    </div>
                  </div>
                </b-modal>
              </div>
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
  .text-wrapper {
    max-width: 670px;
  }

  .text-wrapper h1 {
    max-width: 1100px;
  }
  .text-wrapper h5 {
    max-width: none;
  }
}

@media (min-width: 1400px) {
  .text-wrapper {
    max-width: 900px;
  }
}
</style>
