<template>
<div class="hero">
  <div class="hero-body">
    <slot></slot>
  </div>
</div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'

@Component
export default class Hero extends Vue { }
</script>

<style lang="scss" scoped>
.hero-body {
  padding: 0 0 3rem;
}
</style>
