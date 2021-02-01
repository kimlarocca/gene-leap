<template>
  <div class="programs">
    <div class="hero">
      <div class="hero-text l-container">
        <h1>Our Programs</h1>
      </div>
    </div>
    <div class="l-container secondary-page-body">
      <v-spacer size="hex" />
      <h2>AAV Programs</h2>
      <div class="pipeline labels">
        <div>Discovery</div>
        <div>Pre-Clinical</div>
        <div>Ind-Enabling</div>
        <div>Phase 1/2</div>
        <div>Phase 3</div>
      </div>
      <pipeline header="GLB-2001: Hemophilia" :progress="2" />
      <pipeline header="GLB-2002: Ophthalmology" :progress="2" />
      <pipeline header="GLB-2003: Alzheimer's" :progress="1" />
      <pipeline header="GLB-2004: Undisclosed" :progress="1" />
      <v-spacer size="triple" />
      <h2>mRNA Programs</h2>
      <div class="pipeline labels">
        <div>Discovery</div>
        <div>Pre-Clinical</div>
        <div>Ind-Enabling</div>
        <div>Phase 1/2</div>
        <div>Phase 3</div>
      </div>
      <pipeline header="GLB-2005: Oncology" :progress="1" />
      <pipeline header="GLB-2006: Undisclosed" :progress="1" />
      <pipeline header="GLB-2007: Undisclosed" :progress="1" />
      <v-spacer size="triple" />
      <h2>OLIGO Programs</h2>
      <div class="pipeline labels">
        <div>Discovery</div>
        <div>Pre-Clinical</div>
        <div>Ind-Enabling</div>
        <div>Phase 1/2</div>
        <div>Phase 3</div>
      </div>
      <pipeline header="GLB-2008: Oncology" :progress="2" />
      <pipeline header="GLB-2009: Undisclosed" :progress="1" />
      <pipeline header="GLB-2010: Undisclosed" :progress="1" />
      <v-spacer size="hex" />
    </div>
  </div>
</template>

<script>
import VSpacer from 'vue-evolve/src/components/VSpacer'
import Pipeline from '../components/Pipeline'

export default {
  name: 'Programs',
  components: {
    Pipeline,
    VSpacer
  }
}
</script>

<style lang="scss">
@import "src/assets/settings";

.programs .labels {
  margin-bottom: var(--space-2);
  display: none;
  @media all and (min-width: $medium) {
    display: flex;
  }
}
</style>
