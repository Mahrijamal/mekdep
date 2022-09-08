<template>
  <div class="edit_post">
    <AdminPostForm :card="edit_post" @submit="onSaved" />
  </div>
</template>

<script>
import axios from 'axios'
import AdminPostForm from '@/components/adminPostForm.vue'
export default {
  components: {
    AdminPostForm,
  },
  asyncData(context) {
    return axios
      .get(
        `https://nuxt-post-73233-default-rtdb.firebaseio.com/posts/${context.params.edit_post}.json`
      )
      .then((res) => {
        return {
          edit_post: res.data,
        }
      })
      .catch((e) => console.log(context.error(e)))
  },
methods: {
  onSaved(edit_post){

  }
}

}
</script>

<style>
</style>