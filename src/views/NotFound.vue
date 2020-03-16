<template>
  <div class="notfound">
    <TitleHero title="404 NOT FOUND" subtitle="AIEEEEEEEEE!" />

    <p>お探しのページはありません。</p>
    <p>無いものは無いし、それでも無い物ねだりをするなら <a href="https://github.com/akaregi/fedyya2">GitHub</a> でも覗きやがってください。</p>

    <blockquote>
      <p>いま、ここでは記憶はございません。</p>
      <p class="has-text-grey">― 小佐野賢治・国会答弁より</p>
    </blockquote>

    <blockquote>
      <p>行く川のながれは絕えずして、しかも本の水にあらず。よどみに浮ぶうたかたは、かつ消えかつ結びて久しくとゞまることなし。世の中にある人とすみかと、またかくの如し。</p>
      <p class="has-text-grey">― 鴨長明・方丈記</p>
    </blockquote>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'
import TitleHero from '@/components/TitleHero.vue'

@Component({ components: { TitleHero } })
export default class NotFound extends Vue {
  mounted () {
    document.title = '404 NOT FOUND - fedyya'
  }
}
</script>
