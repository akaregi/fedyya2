<template>
  <footer class="footer content has-text-centered has-text-grey">
    <p>
      <i>fedyya</i> by AKANE AKAGI.
    </p>
    <p class="license">
      Source codes are licensed under
      <a href="https://opensource.org/licenses/BSD-2-Clause">BSD 2-Clause</a>.
    </p>
    <p class="license">
      This site is licensed under
      <a
        href="https://creativecommons.org/licenses/by-nd/4.0/legalcode"
      >Attribution-NoDerivatives 4.0 International</a>.
    </p>
  </footer>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'

@Component
export default class Footer extends Vue { }
</script>

<style lang="scss" scoped>
.footer {
  background: none;
}

.license {
  margin: 0 !important;
}
</style>
