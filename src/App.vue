<template>
  <div id="app">
    <header>
      <span class="logo-text">I'm almost google</span>
      <!-- <div class="logo">
        <img src="./assets/logo.png" alt="">
      </div> -->
      <search></search>
    </header>
    <main>
      <results></results>
    </main>
  </div>
</template>

<script>
import Search from './components/Search.vue'
import Results from './components/Results.vue'

export default {
  name: 'app',
  components: { Search, Results }
}
</script>

<style src="./assets/style.css"></style>
