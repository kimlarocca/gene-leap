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
              altText="Jason Jingxin Zhang, CSO"
              name="Jason Jingxin Zhang, CSO"
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
              altText="Ekambar Kandimalla, Sr. Dir of mRNA chemistry and oligo research"
              name="Ekambar Kandimalla, Sr. Dir of mRNA chemistry and oligo research"
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
              image="/images/team/pengcheng.jpg"
              altText="Pengcheng Zhou, Dir of AAV research"
              name="Pengcheng Zhou, Dir of AAV research"
              layout="horizontal"
          >
            <slot>
              <ul>
                <li>Previously Associate Director at Voyager;</li>
                <li>Project lead of Voyager’s core AAV program;</li>
                <li>Previously instructor at Harvard Medical School.</li>
              </ul>
            </slot>
          </biography-card>
          <biography-card
              image="/images/team/sun.jpg"
              altText="Dr. Sun"
              name="Dr. Sun"
              layout="horizontal"
          >
            <slot>
              <ul>
                <li>15+ years experience of drug delivery system development in pharmaceutical industry. Led the development of multiple products and some of them have been approved or in clinical trials phase;</li>
                <li>PhD from China Pharmaceutical University.</li>
              </ul>
            </slot>
          </biography-card>
          <biography-card
              image="/images/team/wenzhong.jpg"
              altText="Wenzhong Chen"
              name="Wenzhong Chen"
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
<!--        <biography-card-->
<!--            image="/images/team/guangping.jpg"-->
<!--            altText="Prof. Guangping Gao"-->
<!--            name="Prof. Guangping Gao"-->
<!--            layout="horizontal"-->
<!--        >-->
<!--          <slot>-->
<!--            <p>Co-Director, Li Weibo Institute for Rare Diseases Research, Director, Horae Gene Therapy Center and Viral Vector Core, Professor in the University of Massachusetts Medical School.</p>-->
<!--            <v-spacer />-->
<!--            <p>Dr. Gao played a key role in the discovery and characterization of new family of adeno-associated virus (AAV) serotypes, which was instrumental in reviving the gene therapy field. Dr. Gao has published 250+ research papers, holds 131 patents with 221 more pending. Dr. Gao was a co-founder of Voyager Therapeutics.-->
<!--            </p>-->
<!--          </slot>-->
<!--        </biography-card>-->
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
