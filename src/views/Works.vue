<template>
  <div class="works">
    <TitleHero title="Works" subtitle="有耶無耶な何かの紹介" />

  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'
import TitleHero from '@/components/TitleHero.vue'

@Component({ components: { TitleHero } })
export default class Works extends Vue {
  mounted () {
    document.title = 'Works - fedyya'
  }
}
</script>
