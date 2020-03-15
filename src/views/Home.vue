<template>
  <div class="home">
    <TitleHero title="Welcome to fedyya" subtitle="(So take me to tommorow)" />
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'
import TitleHero from '@/components/TitleHero.vue'

@Component({ components: { TitleHero } })
export default class Home extends Vue {
  mounted () {
    document.title = 'Main - fedyya'
  }
}
</script>
