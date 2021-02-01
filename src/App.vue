<template>
  <div>
    <v-spacer />
    <the-header
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
          <the-menu
              ref="menu"
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
          </the-menu>
        </div>
      </template>
    </the-header>
    <v-spacer />
    <router-view />
  </div>
  <the-footer
      company-name="GeneLeap Biotech"
      :navigation="navigation"
  >
    <template v-slot:blurb>
      <p>Unless otherwise specified, all product names appearing on this Internet site are trademarks owned by or licensed to Luye Boston R&D IIC, its subsidiaries or affiliates. No use of any Luye Boston R&D IIC trademark, trade name, or trade dress on this site may be made without the prior written authorization of Luye Boston R&D IIC except to identify the product or services of the company. This Luye Boston R&D IIC website focusing on science is intended for the use of U.S. healthcare professionals any sciences.</p>
    </template>
  </the-footer>
</template>

<script>
import TheHeader from 'vue-evolve/src/components/TheHeader'
import VSpacer from 'vue-evolve/src/components/VSpacer'
import TheFooter from 'vue-evolve/src/components/TheFooter'
import TheMenu from 'vue-evolve/src/components/TheMenu'
import VButton from 'vue-evolve/src/components/VButton'
import SecondaryNavigation from 'vue-evolve/src/components/SecondaryNavigation'

export default {
  name: 'GeneLeap',
  components: {
    TheHeader,
    VSpacer,
    TheFooter,
    TheMenu,
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
