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
            image="/images/team/wenzhong.jpg"
            altText="Dr. Wenzhong Chen, CEO"
            name="Dr. Wenzhong Chen, CEO"
            layout="horizontal"
          >
            <slot>
              <ul>
                <li>20+year experience in scientific research management of pharmaceutical enterprises;</li>
                <li>Expert of liposomal drug development and industrialization.</li>
              </ul>
            </slot>
          </biography-card>
          <biography-card
            image="/images/team/tim.jpg"
            altText="Tim Maguire, CBO, Head of Business Development"
            name="Tim Maguire, CBO, Head of Business Development"
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
            image="/images/team/tomhuang.jpg"
            altText="Tom Huang, COO"
            name="Tom Huang, COO"
            layout="horizontal"
          >
            <slot>
              <ul>
                <li>VP at Luye Life sciences;</li>
                <li>15+ years experience of drug delivery system development in pharmaceutical industry. Led the development of multiple products and some of them have been approved or in clinical trials phase;</li>
                <li>PhD from University of Akron in advance drug delivery.</li>
              </ul>
            </slot>
          </biography-card>
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
        </div>
        <v-spacer size="hex" />
      </div>
    </div>
    <div class="l-container">
      <v-spacer size="hex" />
      <h3>Board of Advisors</h3>
      <div class="l-grid l-grid--2up l-grid--large-gutters">
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
        <biography-card
          image="/images/team/placeholder.png"
          altText="Dr. Bob Langer"
          name="Dr. Bob Langer"
          layout="horizontal"
        >
          <slot>
            <p>Dr. Langer’s pioneering work in the study and development of polymers to deliver drugs, particularly macromolecules, has lead to countless breakthroughs in the filed of biotechnology, and has led to the advancement of countless therapeutics.</p>
            <v-spacer />
            <p>Dr. Langer will advise on the development of delivery platforms for non-messenger RNA therapeutic approaches.</p>
          </slot>
        </biography-card>
        <biography-card
          image="/images/team/placeholder.png"
          altText="Dr. Drew Weissman"
          name="Dr. Drew Weissman"
          layout="horizontal"
        >
          <slot>
            <p>Coming soon.</p>
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
