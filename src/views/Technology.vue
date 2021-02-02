<template>
  <div class="technology">
    <div class="hero">
      <div class="hero-text l-container">
        <h1>Technology</h1>
        <p>We seek to treat patient populations with urgent unmet needs, who currently have no available therapies to modify the progressive course of their disease.</p>
      </div>
    </div>
    <div class="l-container secondary-page-body">
      <v-spacer size="hex" />
      <h2>Our Science</h2>
      <p>Leveraging recent breakthroughs in human genetics and the transformative success of nucleic acid (mRNA and oligo) and AAV-based gene therapy, our goal is to use a precision medicine approach to slow or stop the progression of diseases in the fields of neurodegeneration and oncology, as well as other multiple rare and common indications.</p>
      <v-spacer size="double" />
      <h2>Gene Therapy</h2>
      <p>The goal of gene therapy is to treat or possibly prevent disease. Scientists have been investigating and evolving gene therapy for more than 50 years. One goal of gene therapy research is to determine whether a new or functional gene can be used to restore the function of, or inactivate, a mutated gene.</p>
      <v-spacer size="triple" />
      <div class="technology-cards">
        <div class="l-grid l-grid--3up l-grid--large-gutters">
          <div>
            <v-card
                image="/images/dna.jpg"
                subtitle="DNA"
                description="DNA stores instructions for proteins in the nucleus"
            />
          </div>
          <div>
            <v-card
                image="/images/rna.jpg"
                subtitle="mRNA"
                description="mRNA is a temporary set of instructions for cells to make a protein; mRNA is made using DNA"
            />
          </div>
          <div>
            <v-card
                image="/images/protein.jpg"
                subtitle="Protein"
                description="Proteins form the basis of life by performing the functions required by every cell; proteins are made using mRNA"
            />
          </div>
        </div>
      </div>
      <v-spacer size="hex" />
    </div>
    <div class="u-background-color--gray--light">
      <v-spacer size="hex" />
      <div class="l-container">
        <content-card
            title="Our Three Foci"
            image="/images/technology.jpg"
            alt-text="geneleap biotech technology"
            alignment="right"
            vertical-alignment="middle"
        >
          <p class="u-space--double--bottom">At GeneLeap Biotechnology, we develop highly innovative drugs based on synthetic modified messenger RNA (mRNA). These mRNAs encode virtually any conceivable natural or engineered protein and are designed to be taken up by the cells in specific tissues and organs. We focus on diseases wherein enabling targeted cells to produce – or turn ‘on’ – one or more proteins helping the body to fight or prevent disease.</p>
          <p class="u-space--double--bottom">These synthetic mRNAs are produced with a proprietary manufacturing process. During manufacturing, chemically modified nucleotides other than the natural adenosine, guanosine, uridine, and cytidine can be incorporated into the macromolecule using enzymatic reactions or chemical synthesis. GeneLeap Bio. has a team of very experienced Medicinal Chemists in Woburn and Nanjing working on developing proprietary chemical modifications of mRNA, including 5’-cap, poly-A tail and in the coding region, for improved stability, reduced immunogenicity, and enhanced translation efficacy.</p>
        </content-card>
        <p class="u-space--double--bottom">In some cases, these improvements are combined with sequence alteration of the whole mRNA. The combination of both strategies allows the design of an mRNA to meet its exact purpose, high or low expression levels, temporary or long-lasting expression, strong or undetectable stimulation of the immune system.</p>
        <p class="u-space--double--bottom">The mRNAs are administered into the body as a formulation. This formulation can be a simple buffer or complex nanoparticles to deliver the mRNA into the right cell type. Here we exploit the many years of Luye’s experience in developing drug delivery concepts to the market. Once delivered, the mRNA act as cellular software directing ribosomes to express proteins or antibodies within targeted tissues, and as a consequence, trigger a physiologic benefit for the body and cure diseases.</p>
        <p>At GeneLeap, we are expanding the use of adeno-associated viral (AAV) vectors against strategically selected cell targets, including the retina, liver, and central nervous system. Additionally, we are actively advancing the development of oligonucleotide-based TLR9 agonists for immune-oncology applications allows reduced dosing frequency with improved efficacy for cancer patients with unmet medical needs distinguishing from the current treatments in the clinic.</p>
        <v-spacer size="hex" />
      </div>
    </div>
  </div>
</template>

<script>
import VSpacer from 'vue-evolve/src/components/VSpacer'
import VCard from 'vue-evolve/src/components/VCard'
import ContentCard from 'vue-evolve/src/components/ContentCard'

export default {
  name: 'Technology',
  components: {
    VCard,
    ContentCard,
    VSpacer
  }
}
</script>
