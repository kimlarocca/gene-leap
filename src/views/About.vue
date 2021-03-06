<template>
  <div class="about">
    <div class="hero">
      <div class="hero-text l-container">
        <h1>About Us</h1>
        <p>GeneLeap Biotech is a global gene therapy company in the Luye Life Sciences portfolio of companies, a leader in China and a new entrant in the US. Our goal is to deliver a best-in-class portfolio of completely novel gene therapies.</p>
      </div>
    </div>
    <div class="l-container secondary-page-body">
      <v-spacer size="hex" />
      <h2>Leveraging recent breakthroughs in human genetics</h2>
      <p>GeneLeap Biotech is leveraging recent breakthroughs in human genetics that point to potential disease-modifying targets for these diseases. Our programs utilize a precision medicine approach targeting patient populations with urgent unmet needs, where there are currently no available therapies that modify the progressive course of their disorders.</p>
      <v-spacer size="hex" />
    </div>
    <div class="u-background-color--gray--light">
      <div class="l-container">
        <v-spacer size="hex" />
        <h3>Executive Team</h3>
        <div class="l-grid l-grid--2up l-grid--large-gutters">
          <biography-card
              image="/images/team/ekambar.jpg"
              altText="Ekambar Kandimalla, VP of mRNA chemistry and oligo research"
              name="Ekambar Kandimalla, VP of mRNA chemistry and oligo research"
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
              altText="Tim Maguire, Head of Business Development"
              name="Tim Maguire, Head of Business Development"
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
              image="/images/team/sun.jpg"
              altText="Kaoxiang Sun, VP"
              name="Kaoxiang Sun, VP"
              layout="horizontal"
          >
            <slot>
              <ul>
                <li>VP at Luye Life sciences;</li>
                <li>15+ years experience of drug delivery system development in pharmaceutical industry. Led the development of multiple products and some of them have been approved or in clinical trials phase;</li>
                <li>PhD from China Pharmaceutical University.</li>
              </ul>
            </slot>
          </biography-card>
          <biography-card
              image="/images/team/wenzhong.jpg"
              altText="Wenzhong Chen, Deputy General Manager"
              name="Wenzhong Chen, Deputy General Manager"
              layout="horizontal"
          >
            <slot>
              <ul>
                <li>20+year experience in scientific research management of pharmaceutical enterprises;</li>
                <li>Expert of liposomal drug development and industrialization.</li>
              </ul>
            </slot>
          </biography-card>
        </div>
        <v-spacer size="hex" />
      </div>
    </div>
    <div class="l-container">
      <v-spacer size="hex" />
      <h3>Board of Advisors</h3>
      <div class="l-grid l-grid--2up l-grid--large-gutters">
        <biography-card
            image="/images/team/guangping.jpg"
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
            image="/images/team/herzog.jpg"
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
      <v-spacer size="hex" />
    </div>

    <div class="u-background-color--gray--light">
      <v-spacer size="hex" />
      <div class="l-container">
        <h3>Partners</h3>
        <ul>
          <li>MIT</li>
          <li>Peking University</li>
        </ul>
        <v-spacer size="hex" />
      </div>
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
