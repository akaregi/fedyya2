<template>
  <div class="home">
    <Hero>
      <h1 class="title is-1">fedyya Main Page</h1>
      <h2 class="subtitle is-3">Welcome to <i>fedyya</i></h2>
    </Hero>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'
import Hero from '@/components/Hero.vue'

@Component({ components: { Hero } })
export default class Home extends Vue {
  mounted () {
    document.title = 'Main - fedyya'
  }
}
</script>
