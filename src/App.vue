<template>
  <div id="app">
    <div class="columns is-mobile is-gapless is-centered">
      <div class="column is-half-desktop">
        <b-navbar spaced>
          <template #brand>
            <b-navbar-item>
              <router-link to="/">
                <img
                  class="image"
                  src="https://www.gravatar.com/avatar/6a8bcd15f79dcc2e30138080702b1b09?s=256"
                  alt="akaregi's avatar"
                />
              </router-link>
            </b-navbar-item>
          </template>

          <template #start>
            <b-navbar-item tag="router-link" :to="{ path: '/' }">Home</b-navbar-item>
            <b-navbar-item tag="router-link" :to="{ path: '/about' }">About</b-navbar-item>
            <b-navbar-item tag="router-link" :to="{ path: '/works' }">Works</b-navbar-item>
            <b-navbar-item tag="router-link" :to="{ path: '/links' }">Links</b-navbar-item>
          </template>
        </b-navbar>

        <main class="container content">
          <section class="section">
            <transition appear>
              <router-view />
            </transition>
          </section>
        </main>

        <Footer />
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'
import Footer from '@/components/Footer.vue'

@Component({ components: { Footer } })
export default class App extends Vue { }
</script>

<style lang="scss" scoped>
.v-leave-to, .v-leave-active {
  visibility: collapse;
}

.v-enter-to, .v-enter-active {
  transition: opacity 1s;
}

.v-enter {
  opacity: 0;
}

.router-link-exact-active {
  color: #42b983 !important;
}

a.navbar-item:focus {
  background: none;
  color: #4a4a4a;
}
</style>
