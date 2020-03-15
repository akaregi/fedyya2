<template>
<div class="hero">
  <div class="hero-body">
    <h1 class="title is-1">{{ title }}</h1>
    <h2 class="subtitle is-3">{{ subtitle }}</h2>
  </div>
</div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator'

@Component
export default class Hero extends Vue {
  @Prop({ type: String, required: true, default: 'Untitled' })
  title!: string

  @Prop({ type: String, required: true, default: 'No subtitle' })
  subtitle!: string
}
</script>

<style lang="scss" scoped>
.hero-body {
  padding: 0 0 3rem;
}
</style>
