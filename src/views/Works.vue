<template>
  <div class="works">
    <Hero>
      <h1 class="title is-1">Works</h1>
      <h2 class="subtitle is-3">有耶無耶な何かの紹介</h2>
    </Hero>

  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'
import Hero from '@/components/Hero.vue'

@Component({ components: { Hero } })
export default class Works extends Vue {
  mounted () {
    document.title = 'Works - fedyya'
  }
}
</script>
