<template>
  <div>
    <v-spacer />
    <v-header
        layout="right"
        responsive="true"
    >
      <template v-slot:logo>
        <router-link to="/">
          <img
              src="/images/logo.jpg"
              width="150"
              alt="GeneLeap Bioteach logo"
          />
        </router-link>
      </template>
      <template v-slot:button>
        <router-link to="investors">
          <v-button>
            Investors
          </v-button>
        </router-link>
      </template>
      <template v-slot:navigation>
        <secondary-navigation
            orientation="horizontal"
            :nav-items="navigation"
        />
      </template>
      <template v-slot:menu>
        <div>
          <v-menu
              layout="right"
              :primaryNav="navigation"
          >
            <template v-slot:logo>
              <img
                  src="/images/logo-gray.jpg"
                  width="200"
                  alt="GeneLeap Bioteach logo"
              />
            </template>
            <template v-slot:button>
              <router-link to="investors">
                <v-button>
                  Investors
                </v-button>
              </router-link>
            </template>
            <template v-slot:social>
              <ul class="social-links">
                <social-link
                    icon="fab fa-facebook-f"
                    link="https://www.facebook.com"
                    label="facebook"
                >
                </social-link>
                <social-link
                    icon="fab fa-twitter"
                    link="https://www.twitter.com"
                    label="twitter"
                >
                </social-link>
                <social-link
                    icon="fab fa-youtube"
                    link="https://www.youtube.com"
                    label="youtube"
                >
                </social-link>
                <social-link
                    icon="fab fa-instagram"
                    link="https://www.instagram.com"
                    label="instagram"
                >
                </social-link>
                <social-link
                    icon="fab fa-linkedin-in"
                    link="https://www.linkedin.com"
                    label="linkedin"
                >
                </social-link>
              </ul>
            </template>
          </v-menu>
        </div>
      </template>
    </v-header>
    <v-spacer />
    <router-view />
  </div>
  <v-footer
      company-name="GeneLeap Biotech"
      :navigation="navigation"
  >
    <template v-slot:blurb>
      <p>Unless otherwise specified, all product names appearing on this Internet site are trademarks owned by or licensed to Luye Boston R&D IIC, its subsidiaries or affiliates. No use of any Luye Boston R&D IIC trademark, trade name, or trade dress on this site may be made without the prior written authorization of Luye Boston R&D IIC except to identify the product or services of the company. This Luye Boston R&D IIC website focusing on science is intended for the use of U.S. healthcare professionals any sciences.</p>
    </template>
  </v-footer>
</template>

<script>
import VHeader from 'vue-evolve/src/components/VHeader'
import VSpacer from 'vue-evolve/src/components/VSpacer'
import VFooter from 'vue-evolve/src/components/VFooter'
import VMenu from 'vue-evolve/src/components/VMenu'
import VButton from 'vue-evolve/src/components/VButton'
import SecondaryNavigation from 'vue-evolve/src/components/SecondaryNavigation'

export default {
  name: 'GeneLeap',
  components: {
    VHeader,
    VSpacer,
    VFooter,
    VMenu,
    VButton,
    SecondaryNavigation
  },
  data () {
    return {
      navigation: [
        {
          route: '/about',
          text: 'About',
        },
        {
          route: '/technology',
          text: 'Technology',
        },
        {
          route: '/careers',
          text: 'Careers',
        },
        {
          route: '/programs',
          text: 'Programs',
        },
        {
          route: '/contact',
          text: 'Contact',
        }
      ]
    }
  }
}
</script>
