<template>
  <div class="programs">
    <div class="hero">
      <div class="hero-text l-container">
        <h1>Contact Us</h1>
        <p>GeneLeap is an early start up biotechnology company located in Woburn MA</p>
      </div>
    </div>
    <div class="l-container secondary-page-body">
      <v-spacer size="hex" />
      <div class="l-grid l-grid--2up">
        <div>
          <h2>For General Inquiries, Please Contact Us</h2>
          <p class="u-space--bottom"><a href="mailto:julie.armstrong@luye.com">Email Us</a></p>
          <p>19 Presidential Way</p>
          <p>Woburn MA 01801</p>
          <p>Suite 304</p>
        </div>
        <div class="google-maps">
          <iframe
              src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2940.4467393973864!2d-71.14137818381418!3d42.524564032688346!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x89e30b292dc6f5c3%3A0x417a83779cc3b4fc!2s19%20Presidential%20Way%2C%20Woburn%2C%20MA%2001801!5e0!3m2!1sen!2sus!4v1612131584988!5m2!1sen!2sus"
              width="100%"
              height="600"
              frameborder="0"
              style="border:0;"
              allowfullscreen=""
              aria-hidden="false"
              tabindex="0"
          />
        </div>
      </div>
      <v-spacer size="hex" />
    </div>
  </div>
</template>

<script>
import VSpacer from 'vue-evolve/src/components/VSpacer'

export default {
  name: 'Contact',
  components: {
    VSpacer
  }
}
</script>

<style lang="scss">
@import "src/assets/settings";

.google-maps {
  max-width: 100%;
}
</style>
