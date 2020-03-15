<template>
  <div class="works">
    <Hero>
      <h1 class="title is-1">Works</h1>
      <h2 class="subtitle is-3">有耶無耶な何かの紹介</h2>
    </Hero>

  </div>
</template>

<script lang="ts">
import Hero from '@/components/Hero.vue'

export default {
  mounted: () => {
    document.title = 'Works - fedyya'
  },
  components: {
    Hero
  }
}
</script>
