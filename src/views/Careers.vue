<template>
  <div class="programs">
    <div class="hero">
      <div class="hero-text l-container">
        <h1>Careers</h1>
        <p>GeneLeap is an early start up biotechnology company that specializes in gene therapy areas.</p>
      </div>
    </div>
    <div class="l-container secondary-page-body">
      <v-spacer size="hex" />
      <content-card
          title="Invent, discover, develop, manufacture, commercialize"
          image="/images/careers.jpg"
          alt-text="geneleap biotech careers"
          alignment="left"
          vertical-alignment="middle"
          link="/contact"
          cta="CONTACT US TO LEARN MORE"
      >
        <p>GeneLeap Bio. is an early start-up biotechnology company headquartered in Singapore, with research sites located in Woburn, MA, and Nanjing, China. It is a Luye portfolio company specialized in gene therapy areas. Luye is a leading life science group with R&D sites located in Greater Boston, MA; Princeton, NJ; Nanjing, China; and Yantai, China. Luye invents, discovers, develops, manufactures, and commercializes medicines to treat severe medical conditions for oncology, CNS, metabolism, and other areas of high unmet medical need.</p>
      </content-card>
      <v-spacer size="hex" />
      <div class="careers-cards">
        <h2>Open Positions</h2>
        <div class="l-grid l-grid--4-2-1">
          <v-card
              icon="fas fa-file-word"
              subtitle="Financial Administrator"
              link="/jobs/FinancialAdministrator.docx"
          />
          <v-card
              icon="fas fa-file-word"
              subtitle="Chemist - mRNA Oligonucleotide"
              link="/jobs/mRNAOligonucleotideChemist.pdf"
          />
          <v-card
              icon="fas fa-file-word"
              link="/jobs/InvestigatorI.docx"
              subtitle="Investigator - Analytical / Bioanalytical Chemist"
          />
          <v-card
              icon="fas fa-file-word"
              subtitle="Investigator / Senior Investigator"
              link="/jobs/InvestigatorJD.docx"
          />
          <v-card
              icon="fas fa-file-word"
              subtitle="Project Leader - mRNA"
              link="/jobs/ProjectLeadermRNA.docx"
          />
          <v-card
              icon="fas fa-file-word"
              subtitle="Scientist - mRNA Bioanalytics"
              link="/jobs/ScientistmRNABioanalytics.docx"
          />
          <v-card
              icon="fas fa-file-word"
              subtitle="Scientist - mRNA Downstream Process Development"
              link="/jobs/ScientistDownstream.docx"
          />
          <v-card
              icon="fas fa-file-word"
              subtitle="Scientist - mRNA Early to Late Stage Process Development"
              link="/jobs/ScientistProcessDevelopment.docx"
          />
          <v-card
              icon="fas fa-file-word"
              subtitle="Scientist - Nucleoside Oligonucleotide Purification and Analysis"
              link="/jobs/NucleosideScientist.pdf"
          />
        </div>
      </div>
    </div>
    <v-spacer size="hex" />
  </div>
</template>

<script>
import VCard from 'vue-evolve/src/components/VCard'
import ContentCard from 'vue-evolve/src/components/ContentCard'
import VSpacer from 'vue-evolve/src/components/VSpacer'

export default {
  name: 'Careers',
  components: {
    VCard,
    ContentCard,
    VSpacer
  }
}
</script>
