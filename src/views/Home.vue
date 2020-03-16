<template>
  <div class="home">
    <TitleHero title="Welcome to fedyya" subtitle="(So take me to tommorow)" />

    <h3>Hi</h3>
    <p>ようこそ。ここはトップページなので、上のメニューからいいようにしてください。About は私についてだし、Works は何か出来上がったやつだし、Links はリンク集なので……説明は不要でしょう。 </p>

    <h3>サイトについて</h3>
    <p>このサイトを構成するソースコードはすべて <a href="https://github.com/akaregi/fedyya2">GitHub</a> にあります。このサイト（www.fedyya.net）のライセンスは「<a href="https://creativecommons.org/licenses/by-nd/4.0/deed.ja">クリエイティブ・コモンズ 表示 - 改変禁止 4.0 国際</a>」です。ただし、画像やアイコンは然るべき著作者に権利が帰属します。</p>

    <p>サイト名の <i>fedyya</i> はヒュムノスの単語から来ています。「明日」という意味です。素敵でしょ？ </p>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'
import TitleHero from '@/components/TitleHero.vue'

@Component({ components: { TitleHero } })
export default class Home extends Vue {
  mounted () {
    document.title = 'Home - fedyya'
  }
}
</script>
