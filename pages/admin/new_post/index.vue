<template>
  <div class="new_post_page">
    <h1>Create new post</h1>
    <AdminPostForm @submit12="onSaved" />
  </div>
</template>

<script>
import axios from 'axios'
import AdminPostForm from '@/components/adminPostForm.vue'
export default {
  components: {
    AdminPostForm,
  },
  methods: {
    onSaved(product) {
      axios.post('https://nuxt-post-73233-default-rtdb.firebaseio.com/posts.json', product)
    },
  },
}
</script>

<style>
</style>