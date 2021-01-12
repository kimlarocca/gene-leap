<template>
  <div class="technology">
    <div class="hero">
      <div class="hero-text l-container">
        <h1>Technology</h1>
        <p>We seek to treat patient populations with urgent unmet needs, who currently have no available therapies to modify the progressive course of their disease.</p>
      </div>
    </div>
    <v-spacer size="quad" />
    <div class="l-container">
      <h2>Our Science</h2>
      <p>Leveraging recent breakthroughs in human genetics and the transformative success of mRNA, siRAN, and AAV-based gene therapy, our goal is to use a precision medicine approach to slow or stop the progression of diseases in the fields of neuro-degeneration and oncology, as well as multiple rare indications.</p>
      <v-spacer size="double" />
      <h2>Gene Therapy</h2>
      <p>The goal of gene therapy is to treat or possibly prevent disease. Scientists have been investigating and evolving gene therapy for more than 50 years. One goal of gene therapy research is to determine whether a new or functional gene can be used to restore the function of, or inactivate, a mutated gene.</p>
      <v-spacer size="double" />
      <div class="technology-cards">
        <div class="l-grid l-grid--3up l-grid--large-gutters">
          <div>
            <card
                image="/images/dna.jpg"
                subtitle="DNA"
                description="DNA stores instructions for proteins in the nucleus"
            />
          </div>
          <div>
            <card
                image="/images/rna.jpg"
                subtitle="mRNA"
                description="mRNA is a temporary set of instructions for cells to make a protein; mRNA is made using DNA"
            />
          </div>
          <div>
            <card
                image="/images/protein.jpg"
                subtitle="Protein"
                description="Proteins form the basis of life by performing the functions required by every cell; proteins are made using mRNA"
            />
          </div>
        </div>
      </div>
      <v-spacer size="quad" />
      <content-card
          title="Our Three Foci"
          image="/images/technology.jpg"
          alt-text="geneleap biotech technology"
          alignment="right"
      >
        <template v-slot:content>
          <p>At GeneLeap Biotechnology, we pursue programs using messenger RNA (mRNA) to develop a new class of medicines. we are leveraging the fundamental role that mRNA plays in protein synthesis. We have developed proprietary technologies and methods to create mRNA sequences that cells recognize as if they were produced in the body. We focus on diseases where enabling targeted cells to produce – or turn ‘on’ – one or more given proteins will enable the body to fight or prevent a given disease.</p>
          <p>Additionally, we are advancing the use of using adeno-associated viral (AAV) vectors to advance research programs against strategically selected cell targets, for example, the retina, liver and central nervous system.</p>
        </template>
      </content-card>
      <p>Our newest area of development is in non-coding RNAs, enabling RNA interference or RNAi, as it is termed in the biotech field. Therapeutics in this realm of research and development include modalities such as small interfering RNAs (siRNAs) and microRNAs (miRNAs). They provide amazing potential in a variety of ways:</p>
      <ol>
        <li>The ability to harness a natural pathway.</li>
        <li>The ability to target virtually any protein.</li>
        <li>Acting as “upstream switches” of today’s medicines.</li>
        <li>Simplifying and accelerating the discovery of drug candidates.</li>
      </ol>
      <v-spacer size="quad" />
    </div>
  </div>
</template>

<script>
import VSpacer from 'vue-evolve/src/components/VSpacer'
import Card from 'vue-evolve/src/components/Card'
import ContentCard from 'vue-evolve/src/components/ContentCard'

export default {
  name: 'Technology',
  components: {
    Card,
    ContentCard,
    VSpacer
  }
}
</script>

<style lang="scss">
@import "src/assets/settings";

</style>
