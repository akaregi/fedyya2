<template>
  <div class="box">
      <a v-bind:href="url">
        <h4>{{ title }}</h4>
      <p class="has-text-grey-light">{{ lead }}</p>
      </a>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator'

@Component
export default class LinkBox extends Vue {
  @Prop({ type: String, required: true, default: 'Untitled' })
  title!: string

  @Prop({ type: String, required: true, default: 'No lead' })
  lead!: string

  @Prop({ type: String, required: false, default: '' })
  url!: string
}
</script>

<style lang="scss" scoped>
@mixin newBoxColor($x, $y, $z, $hoverX: 66, $hoverY: 185, $hoverZ: 131) {
  box-shadow: 0 .5em 1em -.1em rgba($x, $y, $z, .2), 0 0 0 1px rgba($x, $y, $z, .02);
  border: 1px solid rgba($x, $y, $z, .1);

  &:hover {
    box-shadow: 0 .5em 1em -.1em rgba($hoverX, $hoverY, $hoverZ, .2), 0 0 0 1px rgba($hoverX, $hoverY, $hoverZ, .02);
    border: 1px solid rgba($hoverX, $hoverY, $hoverZ, 1);
  }
}

a {
  display: block;

  padding: 1.25rem;
}

.box {
  transition: .5s;

  padding: 0;

  @include newBoxColor(100, 100, 100);
}

.is-twitter {
  @include newBoxColor(29, 161, 242);
}

.is-mastodon {
  @include newBoxColor(43, 144, 217);
}

.is-scrapbox {
  @include newBoxColor(6, 183, 50);
}
</style>
