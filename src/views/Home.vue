<template>
  <div class="home">
    <div class="hero">
      <div class="hero-text l-container">
        <h1>Completely Novel Gene Therapies</h1>
        <p>GeneLeap Biotech is a global gene therapy company in the Luye Lifesciences portfolio of companies, a leader in China and a new entrant in the US. Our goal is to deliver a best-in-class portfolio of completely novel gene therapies.</p>
      </div>
    </div>
    <div class="home-cards">
      <div class="l-container l-grid l-grid--3up l-grid--large-gutters">
        <div>
          <card
              icon="fas fa-globe"
              subtitle="global excellence"
              description="Global centers of excellence for GMP and Commercial manufacturing"
          />
        </div>
        <div>
          <card
              icon="fas fa-dna"
              subtitle="history & experience"
              description="A long history of novel drug delivery experience and marketed products"
          />
        </div>
        <div>
          <card
              icon="fas fa-file-medical"
              subtitle="stellar record"
              description="A stellar record with the FDA (over 10 years) and CFDA (over 25 years)"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Card from 'vue-evolve/src/components/Card'

export default {
  name: 'Home',
  components: {
    Card
  }
}
</script>

<style lang="scss">
@import "src/assets/settings";

.home .hero {
  background: black url("/images/home-hero.jpg") no-repeat left -100px top;
  @media all and (min-width: $medium) {
    background: black url("/images/home-hero.jpg") no-repeat left top;
  }
  @media all and (min-width: $xlarge) {
    background: black url("/images/home-hero.jpg") no-repeat right top;
  }
}

.home .home-cards {
  position: relative;
  background: white url("/images/home-cards-background.jpg") no-repeat left top;
  padding: var(--space-10) var(--space-4);
  min-height: 480px;
  @media all and (min-width: $medium) {
    padding: var(--space-10) 0;
  }
}
</style>
