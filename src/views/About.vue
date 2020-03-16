<template>
  <div class="about">
    <TitleHero title="About the author" subtitle="「あかれぎ」の真相に迫る" />

    <figure class="image">
      <img class="is-rounded" src="https://www.gravatar.com/avatar/6a8bcd15f79dcc2e30138080702b1b09?s=256" alt="akaregi's avatar">
      <figcaption class="has-text-grey">The cute icon from <a href="https://twitter.com/Shishamo_4096">@Shishamo_4096</a></figcaption>
    </figure>

    <h3>お名前は？</h3>
    <p><strong>あかれぎ</strong>。 <i>akaregi</i> とも。こっちのローマ字表記は小文字。</p>
    <p>万が一普通の名前を使う他ない、まさに由々しき事態に遭遇したら「赤城 茜」という名を使う。ローマ字表記で <i>AKANE AKAGI</i> 。こっちのローマ字表記は大文字。</p>
    <p>ほか、ゲームでは <i>AkagiCrafter</i> など別の名前を使うことがある。</p>

    <h3>もうちょっと詳しく</h3>
    <p>三月生まれ、群馬県前橋市出身……そのぐらい？</p>

    <h3>趣味はなんぞや</h3>
    <p>暇な時間は何かしらゲームをしているか寝ている。ゲームしつつ寝る凶行もしてがす。たまにプログラミングもするが、まあその……趣味で独学の範疇だから。</p>

    <h3>接触を図りたい</h3>
    <p>Twitter なら <a href="https://twitter.com/akgmoegi">@akgmoegi</a>、Discord なら「あかれぎ#8089」でお願いします。物理的な接触は、その、個人情報は（あまり）漏らさない主義ですので、ご理解ください……。</p>

    <hr>

    <h3>結論</h3>
    <blockquote>
      <p>そうか、そうか、つまり君はそんなやつなんだな。</p>
      <p class="has-text-grey">― ヘルマン・ヘッセ「少年の日の思い出」</p>
    </blockquote>

    <p>アーハン率100%になりました？</p>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'
import TitleHero from '@/components/TitleHero.vue'

@Component({ components: { TitleHero } })
export default class About extends Vue {
  mounted () {
    document.title = 'About - fedyya'
  }
}
</script>

<style lang="scss" scoped>
figure {
  &.image img {
    width: auto;

    margin-left: auto;
    margin-right: auto;
  }

  & figcaption {
    text-align: center;
  }
}
</style>
