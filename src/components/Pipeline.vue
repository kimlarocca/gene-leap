<template>
  <div class="pipeline-header">
    <h4>{{ header }}</h4>
  </div>
  <div class="pipeline">
    <div :class="progress>0 ? 'u-background-color--quinary' : ''">
      <div
          v-if="progress===1"
          class="pipeline-label"
      >Discovery
      </div>
    </div>
    <div :class="progress>1 ? 'u-background-color--quinary' : ''">
      <div
          v-if="progress===2"
          class="pipeline-label"
      >Pre-Clinical
      </div>
    </div>
    <div :class="progress>2 ? 'u-background-color--quinary' : ''">
      <div
          v-if="progress===3"
          class="pipeline-label"
      >IND-Enabling
      </div>
    </div>
    <div :class="progress>3 ? 'u-background-color--quinary' : ''">
      <div
          v-if="progress===4"
          class="pipeline-label"
      >Phase 1/2
      </div>
    </div>
    <div :class="progress>4 ? 'u-background-color--quinary' : ''">
      <div
          v-if="progress===5"
          class="pipeline-label"
      >Phase 3
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Pipeline',
  props: {
    header: String,
    progress: {
      type: Number,
      default: 0
    },
  }
}
</script>

<style lang="scss">
@import "src/assets/settings";

.pipeline-header {
  background-color: var(--color-light-gray);
  padding: var(--space-2);
}

.pipeline {
  display: flex;
  text-align: center;
  color: var(--color-primary);
  margin-bottom: var(--space-2);
  position: relative;

  div {
    padding: var(--space-2);
    flex-basis: 20%;
    min-height: 43px;
    font-weight: 800;
    text-transform: uppercase;
  }
}

.pipeline-label {
  position: absolute;
  top: 0;
  left: 0;
  font-size: var(--font-size-4);
  @media all and (min-width: $large) {
    display: none;
  }
}
</style>
