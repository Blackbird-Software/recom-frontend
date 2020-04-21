<template>
  <b-container fluid>

    <navbar></navbar>

    <book-list></book-list>

  </b-container>
</template>

<script lang="ts">
  import Vue from 'vue'
  import Navbar from '~/components/Navbar.vue'
  import BookList from '~/components/BookList.vue'

  export default Vue.extend({
    components: {
      Navbar,
      BookList
    }
  })
</script>
