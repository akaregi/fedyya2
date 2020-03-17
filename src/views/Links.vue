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

    <hr>

    <h3>いぇーい</h3>

    <b-notification>
      <p>🔗 リンク先の方へ： 上のソーシャルメディア的な色付けをご所望でしたらご連絡ください。</p>
    </b-notification>

    <b-notification>
      <p>括弧内は作者名です（敬称略）。</p>
    </b-notification>

    <h4>一般</h4>
    <LinkBox
      title="みことはねっと（兎月くみ）"
      lead="スラヴ語派（？）のやべーやつのご登場だ！人たらし（自認）だけどいい人だよ"
      url="https://mikotoha.net"
    />

    <LinkBox
      title="Escapism（にらり）"
      lead="お絵かきとかタロットとか色々しているらしい。書いて思ったけどよく知らない……！"
      url="https://www.escapism.work"
    />

    <LinkBox
      title="homepage（nagiko）"
      lead="上のマストドンサーバ管理者のページ。足を向けて寝られない。"
      url="https://bananagikoh.github.io/homepage/pages/mastodon-use/profile.html"
    />

    <h4>Scrapbox</h4>
    <LinkBox
      class="is-scrapbox"
      title="mikura-knowledge（かるま）"
      lead="Lorem ipsum dolor sit amet, consectetur adipiscing elit."
      url="https://scrapbox.io/mikura-knowledge/"
    />

    <LinkBox
      class="is-scrapbox"
      title="hakobe-public（はこべ）"
      lead="植物のやべーやつだ！べっちだったりべっちゃんこだったり異名が多い。"
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

<style lang="scss" scoped>
hr {
  margin: 3rem 0;
}
</style>
