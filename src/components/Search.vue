<template lang="html">
  <div class="Search">
    <input type="text" class="Search__input" v-model="query" @keyup.enter="search()">
    <button class="Search__button" @click="search()">FIND</button>
  </div>
</template>

<script>

export default {
  data() {
    return {
      query: ''
    }
  },
  methods: {
    search() {
      //вместо обычной переменной store 'store.dispatch('search', this.query)' делаем ее глобальной
      this.$store.dispatch('search', this.query)
    }
  }
}
</script>
