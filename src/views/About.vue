<template>
  <div class="about">
    <Hero>
      <h1 class="title is-1">About the author</h1>
      <h2 class="subtitle is-3">「あかれぎ」の真相に迫る</h2>
    </Hero>

    <figure class="image">
      <img class="is-rounded" src="https://www.gravatar.com/avatar/6a8bcd15f79dcc2e30138080702b1b09?s=256" alt="akaregi's avatar">
      <figcaption class="has-text-grey">The cute icon from <a href="https://twitter.com/Shishamo_4096">@Shishamo_4096</a></figcaption>
    </figure>

    <h3>名前</h3>
    <p><strong>あかれぎ</strong>。 <i>akaregi</i> とも。こっちのローマ字表記は小文字。</p>
    <p>万が一普通の名前を使う他ない、まさに由々しき事態に遭遇したら「赤城 茜」という名を使う。ローマ字表記で <i>AKANE AKAGI</i> 。こっちのローマ字表記は大文字。</p>
    <p>ほか、ゲームでは <i>AkagiCrafter</i> など別の名前を使うことがある。</p>

    <h3>日々の生活</h3>
    <p>人間生活に決まっている。</p>

    <h3>趣味</h3>
    <p>暇な時間は何かしらゲームをしているか寝ている。ゲームしつつ寝る凶行もしてがす。たまにプログラミングもするが、まあその……趣味で独学の範疇だから……。</p>

    <h4>やってるゲーム</h4>
    <ul>
      <li>Euro Truck Simulator 2</li>
      <li>Kerbal Space Program</li>
      <li>各種 Zachtronics ゲー（SHENZHEN I/O, TIS-100, Opus Magnum, MOLEK-SYNTEZ）</li>
      <li>その他色々</li>
    </ul>

    <hr>

    <h3>結論</h3>
    <blockquote>
      <p>そうか、そうか、つまり君はそんなやつなんだな。</p>
    </blockquote>
    <p class="has-text-grey">― ヘルマン・ヘッセ「少年の日の思い出」</p>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'
import Hero from '@/components/Hero.vue'

@Component({ components: { Hero } })
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
