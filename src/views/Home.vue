<template>
  <div class="home l-container">
    <div class="l-grid l-grid--2up l-grid--middle">
      <h1>Completely Novel Gene Therapies</h1>
      <p>GeneLeap Biotech is a global gene therapy company in the Luye Lifesciences portfolio of companies, a leader in China and a new entrant in the US. Our goal is to deliver a best-in-class portfolio of completely novel gene therapies.</p>
    </div>
    <div class="home-hero">
      <div class="home-hero-circle" />
      <img
          src="/images/home-hero.jpg"
          alt="GeneLeap Bioteach, a global gene therapy company"
      />
    </div>
    <v-spacer size="quin" />
    <div class="home-cards l-container l-grid l-grid--3up l-grid--large-gutters">
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
</template>

<script>
import Card from 'vue-evolve/src/components/Card'
import VSpacer from 'vue-evolve/src/components/VSpacer'

export default {
  name: 'Home',
  components: {
    Card,
    VSpacer
  }
}
</script>

<style lang="scss">
@import "src/assets/settings";
.home {
  position: relative;
  &::after {
    display: none;
    @media all and (min-width: $medium) {
      display: block;
      position: absolute;
      top: 0;
      right: -320px;
      content: '';
      height: 300px;
      width: 300px;
      border-radius: 50%;
      background: var(--color-quaternary);
      background: linear-gradient(180deg, var(--color-white) 0%, var(--color-tertiary) 50%, var(--color-tertiary) 100%);
    }
  }
}
.home .home-hero {
  width: 100%;
  margin-top: var(--space-6);
  @media all and (min-width: $medium) {
    margin-top: var(--space-10);
  }
}

.home .home-hero-circle {
  position: relative;
  height: 100px;
  overflow: hidden;

  &::before {
    content: '';
    position: absolute;
    top: 0;
    right: 32px;
    height: 300px;
    width: 300px;
    border-radius: 50%;
    background: var(--color-primary);
    background: linear-gradient(90deg, var(--color-quinary) 0%, var(--color-primary) 100%);
    @media all and (min-width: $medium) {
      right: unset;
      left: 100px;
      height: 400px;
      width: 400px;
    }
  }
}

.home .home-cards {
  text-align: center;
  position: relative;
  &::after {
    position: absolute;
    z-index: -1;
    top: -50px;
    left: -150px;
    content: '';
    height: 400px;
    width: 400px;
    border-radius: 50%;
    background: var(--color-quaternary);
    background: linear-gradient(135deg, var(--color-white) 0%, var(--color-quinary) 75%, var(--color-quinary) 100%);
  }

  .card {
    box-shadow: 0px 0px 20px 0px rgba(0, 0, 0, 0.2);

    .subtitle {
      text-transform: uppercase;
    }
  }

  i {
    font-size: 2rem;
    color: var(--color-secondary);
  }
}
</style>
