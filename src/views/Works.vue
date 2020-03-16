<template>
  <div class="works">
    <TitleHero title="Works" subtitle="有耶無耶な何かの紹介" />

    <h3><a href="https://fedyya.wordpress.com">fedyya BLOG</a>: 三日坊主のブログ</h3>
    <p>名前の通りブログでございます。滅多に書かない。以前のサイト（<code>blog.fedyya.net</code>）は死にました。</p>

    <h3><a href="https://lunaris.fedyya.net">fedyya LUNARIS</a>: ヒュムノスの詩倉庫</h3>
    <p>某ゲームの架空言語「ヒュムノス」で紡いだ詩の倉庫でございます。えらく数が多い。</p>

    <h3><a href="https://rhei.fedyya.net">fedyya RHEI</a>: 納屋</h3>
    <p>納屋です。</p>

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
