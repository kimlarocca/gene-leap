<template>
  <div class="home">
    <div class="home-hero">
      <div class="home-hero-text l-container">
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
  display: flex;
  width: 100%;
  text-align: right;
  min-height: 600px;
  background: black url("/images/home-hero.jpg") no-repeat left -100px top;
  background-size: cover;
  @media all and (min-width: $medium) {
    background: black url("/images/home-hero.jpg") no-repeat left top;
  }
  @media all and (min-width: $xlarge) {
    background: black url("/images/home-hero.jpg") no-repeat right top;
  }
}

.home .home-hero-text {
  color: white;
  text-align: left;
  padding: var(--space-2) 0;

  h1 {
    color: white;
    max-width: 500px;
    margin-bottom: var(--space-4);
    text-shadow: 0 0 30px #000;
  }

  p {
    max-width: 800px;
    font-size: 1.25rem;
    font-weight: 600;
    line-height: 1.5;
    text-shadow: 0 0 30px #000;
  }
}

.home .home-cards {
  text-align: center;
  position: relative;
  background: white url("/images/home-cards-background.jpg") no-repeat left top;
  padding: var(--space-10) var(--space-4);
  min-height: 480px;
  @media all and (min-width: $medium) {
    padding: var(--space-10) 0;
  }

  .card {
    box-shadow: 0px 0px 20px 0px rgba(0, 0, 0, 0.2);
    padding: var(--space-4) 0;

    &:hover {
      opacity: 1;
      box-shadow: 0px 0px 20px 0px rgba(0, 0, 0, 0.4);
    }

    .subtitle {
      text-transform: uppercase;
    }
  }

  i {
    font-size: 2rem;
    color: var(--color-black);
  }
}
</style>
