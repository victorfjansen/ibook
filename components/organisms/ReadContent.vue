<template>
  <div class="container">
    <h2>{{ $book.title }}</h2>

    <ReadSwipperContainer />
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import { books } from '@/store'

export default Vue.extend({
  computed: {
    $book() {
      return books.$single
    },
  },
})
</script>

<style scoped>
.container h2 {
  font-weight: 500;
  margin-bottom: 20px;
}
</style>
