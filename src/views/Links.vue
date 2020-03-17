<template>
  <div class="links">
    <TitleHero title="Links" subtitle="外部サイトへのリンク集" />

    <h3>あかれぎ関連</h3>
    <LinkBox
      class="is-twitter"
      title="Twitter"
      lead="あかれぎのツイッターアカウントです。"
      url="https://twitter.com/akgmoegi"
    />

    <LinkBox
      class="is-mastodon"
      title="Mastodon"
      lead="いつもいるのはこっちの方。"
      url="https://felesitas.cloud/@akane"
    />

    <h3>いぇーい</h3>

    <div class="notification">
      <p>🔗 リンク先の方へ： 上のソーシャルメディア的な色付けをご所望でしたらご連絡ください。</p>
    </div>

    <div class="notification">
      <p>括弧内は作者名です（敬称略）。</p>
    </div>

    <h4>一般</h4>
    <LinkBox
      title="みことはねっと（兎月くみ）"
      lead=""
      url="https://mikotoha.net"
    />

    <LinkBox
      title="Escapism（にらり）"
      lead=""
      url="https://www.escapism.work"
    />

    <LinkBox
      title="homepage（nagiko）"
      lead=""
      url="https://bananagikoh.github.io/homepage/pages/mastodon-use/profile.html"
    />

    <h4>Scrapbox</h4>
    <LinkBox
      class="is-scrapbox"
      title="mikura-knowledge（かるま）"
      lead=""
      url="https://scrapbox.io/mikura-knowledge/"
    />

    <LinkBox
      class="is-scrapbox"
      title="hakobe-public（はこべ）"
      lead=""
      url="https://scrapbox.io/hakobe-public/ "
    />
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'

import LinkBox from '@/components/LinkBox.vue'
import TitleHero from '@/components/TitleHero.vue'

@Component({ components: { TitleHero, LinkBox } })
export default class Links extends Vue {
  mounted () {
    document.title = 'Links - fedyya'
  }
}
</script>
