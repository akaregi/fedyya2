<template>
  <div class="links">
    <Hero>
      <h1 class="title is-1">Links</h1>
      <h2 class="subtitle is-3">外部サイトへのリンク集</h2>
    </Hero>

    <h3>あかれぎ関連</h3>

    <h3>それ以外</h3>

  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'
import Hero from '@/components/Hero.vue'

@Component({ components: { Hero } })
export default class Links extends Vue {
  mounted () {
    document.title = 'Links - fedyya'
  }
}
</script>
