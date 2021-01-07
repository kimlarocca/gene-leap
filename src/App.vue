<template>
  <div class="l-container">
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
    </v-header>
    <v-spacer size="hex" />
    <router-view />
    <v-spacer size="hex" />
  </div>
  <v-footer
      company-name="GeneLeap Biotech"
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

export default {
  name: 'GeneLeap',
  components: {
    VHeader,
    VSpacer,
    VFooter
  }
}
</script>
