<template>
  <BookDetailsTemplate />
</template>

<script lang="ts">
import Vue from 'vue'
import { books } from '@/store'

export default Vue.extend({
  async asyncData({ route, error }) {
    try {
      await books.show({ id: route.params.id as any })
    } catch {
      return error({ statusCode: 404 })
    }
  },
  layout: 'ibook',
  head() {
    return {
      title: books.$single.title,
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: books.$single.description,
        },
      ],
    }
  },
})
</script>

<style scoped></style>
