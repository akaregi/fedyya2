<template>
  <div class="links">
    <TitleHero title="Links" subtitle="外部サイトへのリンク集" />

    <h3>あかれぎ関連</h3>

    <h3>それ以外</h3>

  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'
import TitleHero from '@/components/TitleHero.vue'

@Component({ components: { TitleHero } })
export default class Links extends Vue {
  mounted () {
    document.title = 'Links - fedyya'
  }
}
</script>
