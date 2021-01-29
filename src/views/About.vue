<template>
  <div class="about">
    <div class="hero">
      <div class="hero-text l-container">
        <h1>About Us</h1>
        <p>At GeneLeap Biotech, we are developing a pipeline of gene therapies to slow or stop the underlying disease process for patients in a variety of indications and disorders.</p>
      </div>
    </div>
    <v-spacer size="quad" />
    <div class="l-container">
      <h2>Leveraging recent breakthroughs in human genetics</h2>
      <p>GeneLeap Biotech is leveraging recent breakthroughs in human genetics that point to potential disease-modifying targets for these diseases. Our programs utilize a precision medicine approach targeting patient populations with urgent unmet needs, where there are currently no available therapies that modify the progressive course of their disorders.</p>
      <v-spacer size="quad" />
      <h3>Executive Team</h3>
      <div class="l-grid l-grid--2up l-grid--large-gutters">
        <biography-card
            image="/images/team/sean.jpg"
            altText="Xi-Yong Sean Fu, CEO"
            name="Xi-Yong Sean Fu, CEO"
            layout="horizontal"
        >
          <slot>
            <ul>
              <li>20+ year veteran in the BioPharma industry;</li>
              <li>16 years at Merck & Co., several products on the market, led multiple M&A deals including the merger with Schering-Plough;</li>
              <li>PhD from The Ohio State University, MBA from Wharton School of Business, University of Pennsylvania.</li>
            </ul>
          </slot>
        </biography-card>
        <biography-card
            image="/images/team/matthias.jpg"
            altText="Matthias John, Sr. Dir of mRNA Research"
            name="Matthias John, Sr. Dir of mRNA Research"
            layout="horizontal"
        >
          <slot>
            <ul>
              <li>Previously Research Fellow at Crispr Therapeutics, Senior Research Fellow at Moderna, Associate Director at Roche and Alnylam;</li>
              <li>Experts in therapeutic Crispr, mRNA and siRNA technologies;</li>
            </ul>
          </slot>
        </biography-card>
        <biography-card
            image="/images/team/zhang.jpg"
            altText="Jingxin Jason Zhang, CSO"
            name="Jingxin Jason Zhang, CSO"
            layout="horizontal"
        >
          <slot>
            <ul>
              <li>15+ years’drug discovery and development experiences, previously Senior Dir Wave Life Sciences, Sanofi and Novartis;</li>
              <li>PhD in immunology from NYU; PhD in medicinal chemistry from Peking Union Medical College;</li>
            </ul>
          </slot>
        </biography-card>
        <biography-card
            image="/images/team/ekambar.jpg"
            altText="Ekambar Kandimalla, Sr. Dir of Oligo Rsearch"
            name="Ekambar Kandimalla, Sr. Dir of Oligo Rsearch"
            layout="horizontal"
        >
          <slot>
            <ul>
              <li>Previously CSO at Exicure; VP Idera;</li>
              <li>World’s leading scholar on nucleic acid chemistry;</li>
              <li>Broad experiences in siRNA and SNA therapeutic development;</li>
              <li>Moved multiple candidates into clinical trials.</li>
            </ul>
          </slot>
        </biography-card>
        <biography-card
            image="/images/team/tim.jpg"
            altText="Tim Maguire, BD Head"
            name="Tim Maguire, BD Head"
            layout="horizontal"
        >
          <slot>
            <ul>
              <li>15 yr experiences in VC space;</li>
              <li>CEO / COO of multiple start up companies with multiple successful exits;</li>
              <li>PhD in Bioengineering from Rutgers.</li>
            </ul>
          </slot>
        </biography-card>
        <biography-card
            image="https://via.placeholder.com/320/320?text=coming soon"
            altText="Jing Zhu, Sr. Investigator, Process Development"
            name="Jing Zhu, Sr. Investigator, Process Development"
            layout="horizontal"
        >
          <slot>
            <ul>
              <li>Previously R&D manager at Thermo Fisher;</li>
              <li>Broad experiences in mRNA process developments.</li>
            </ul>
          </slot>
        </biography-card>
      </div>
      <v-spacer size="quad" />
      <h3>Board of Advisors</h3>
      <div class="l-grid l-grid--2up l-grid--large-gutters">
        <biography-card
            image="https://via.placeholder.com/320/320?text=coming soon"
            altText="Prof. Guangping Gao"
            name="Prof. Guangping Gao"
            layout="horizontal"
        >
          <slot>
            <p>Co-Director, Li Weibo Institute for Rare Diseases Research, Director, Horae Gene Therapy Center and Viral Vector Core, Professor in the University of Massachusetts Medical School.</p>
            <v-spacer />
            <p>Dr. Gao played a key role in the discovery and characterization of new family of adeno-associated virus (AAV) serotypes, which was instrumental in reviving the gene therapy field. Dr. Gao has published 250+ research papers, holds 131 patents with 221 more pending. Dr. Gao was a co-founder of Voyager Therapeutics.
            </p>
          </slot>
        </biography-card>
        <biography-card
            image="https://via.placeholder.com/320/320?text=coming soon"
            altText="Prof. Roland W. Herzog"
            name="Prof. Roland W. Herzog"
            layout="horizontal"
        >
          <slot>
            <p>Professor of Pediatrics, Riley Children‘s Foundation Professor of Immunology, and Director of the Gene and Cell Therapy Program. World’s leading exper in gene therapy and immune tolerance for hemophilia and in AAV vectors.</p>
            <v-spacer />
            <p>Dr. Herzog’s research was recognized by awards from American Society of Gene and Cell Therapy, the National Hemophilia Foundation, the Bayer Hemophilia Program, and the University of Florida Research Foundation, among others. Dr. Herzog served on SAB of Sparks Therapeutics.</p>
          </slot>
        </biography-card>
      </div>
      <v-spacer size="quad" />
      <h3>Partners</h3>
      <ul>
        <li>MIT</li>
        <li>Peking University</li>
      </ul>
      <v-spacer size="quad" />
    </div>
  </div>
</template>

<script>
import BiographyCard from 'vue-evolve/src/components/BiographyCard'
import VSpacer from 'vue-evolve/src/components/VSpacer'

export default {
  name: 'About',
  components: {
    BiographyCard,
    VSpacer
  }
}
</script>

<style lang="scss">
@import "src/assets/settings";

</style>
