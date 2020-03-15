<template>
  <div id="app">
    <div class="columns is-mobile is-gapless is-centered">
      <div class="column is-half-desktop">
        <b-navbar>
          <template slot="brand">
            <b-navbar-item>
              <router-link to="/">
                <img
                  src="https://www.gravatar.com/avatar/6a8bcd15f79dcc2e30138080702b1b09?s=110"
                  alt="akaregi's avatar"
                />
              </router-link>
            </b-navbar-item>
          </template>

          <template slot="start">
            <b-navbar-item  tag="router-link" :to="{ path: '/' }">Home</b-navbar-item>
            <b-navbar-item  tag="router-link" :to="{ path: '/about' }">About</b-navbar-item>
            <b-navbar-item  tag="router-link" :to="{ path: '/link' }">Link</b-navbar-item>
          </template>
        </b-navbar>

        <main class="container">
          <section class="section">
            <router-view />
          </section>
        </main>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
export default { }
</script>

<style lang="scss" scoped>
.router-link-exact-active {
  color: #42b983 !important;
}

a.navbar-item:focus {
  background: none;
  color: #4a4a4a;
}
</style>
