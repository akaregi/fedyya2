<template>
  <div class="works">
    <TitleHero title="Works" subtitle="有耶無耶な何かの紹介" />

    <h3>Lianiis Min: 月生まれたちの言葉（サイト作成）</h3>
    <figure>
      <img src="../assets/lianiis.png" alt="Lianiis Min's page">
      <figcaption class="has-text-grey">頑張って作りました</figcaption>
    </figure>

    <p>フルスクラッチで書いたサイトです。<i><a href="https://www.lianiis.com/">Lianiis Min</a></i> とは猫が話す言葉をイメージして作られた人工言語だそうです。</p>

    <hr>

    <h3><a href="https://fedyya.wordpress.com">fedyya BLOG</a>: 三日坊主のブログ</h3>
    <p>名前の通りブログでございます。滅多に書かない。以前のサイト（blog.fedyya.net）は死にました。</p>

    <h3><a href="https://lunaris.fedyya.net">fedyya LUNARIS</a>: ヒュムノスの詩倉庫</h3>
    <p>某ゲームの架空言語「ヒュムノス」で紡いだ詩の倉庫です。<a href="https://github.com/akaregi/Lunaris">GitHub</a> にすべてのソースコードが転がっています。</p>

    <h3><a href="https://rhei.fedyya.net">fedyya RHEI</a>: 納屋</h3>
    <p>納屋 。</p>

    <hr>

    <h3><a href="https://emoji.fedyya.net">Emoji Builder</a>: <i>The Enigmatic Emoji Mechanism</i></h3>
    <p>極めて限定された特定目的において有用な絵文字加工装置でございます。</p>
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
