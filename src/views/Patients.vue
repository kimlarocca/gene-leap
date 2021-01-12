<template>
  <div class="patients">
    <div class="hero">
      <div class="hero-text l-container">
        <h1>Our Patients</h1>
        <p>GeneLeap Biotech is committed to developing safe and effective medicines and treatments for patients worldwide.</p>
      </div>
    </div>
    <v-spacer size="quad" />
    <div class="l-container">
      <h2>Enrolling in GeneLeap Biotech’s clinical trials</h2>
      <p>Before marketing drugs to patients, GeneLeap Biotech designs and conducts clinical trials to generate valid scientific evidence and to protect the rights, safety, and welfare of research participants.</p>
      <p>Enrolling in GeneLeap Biotech’s clinical trials is the primary way that patients who seek access to GeneLeap Biotech’s investigational drug(s) may receive those drug(s). Information about GeneLeap Biotech’s ongoing clinical trials will be found on www.ClinicalTrials.gov by searching “GeneLeap Biotech” in the “sponsor” field under the heading “Advanced Search.”</p>
      <p>“Expanded access” and “compassionate use” are processes through which a patient and the patient’s physician may seek to obtain an investigational product outside of a clinical trial. These programs only apply to medicines not yet approved by the national drug regulatory authority in the country of the patient’s residence.</p>
      <p>GeneLeap Biotech evaluates expanded access and compassionate use requests on an individual basis. GeneLeap Biotech may revise this policy at any time.</p>
    </div>
    <v-spacer size="quad" />
  </div>
</template>

<script>
import VSpacer from 'vue-evolve/src/components/VSpacer'

export default {
  name: 'Patients',
  components: {
    VSpacer
  }
}
</script>

<style lang="scss">
@import "src/assets/settings";
</style>
