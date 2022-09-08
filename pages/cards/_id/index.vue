<template>
  <div class="card_info">
    <h1>{{ loadedPosts }}</h1>
  </div>
</template>

<script>
import axios from 'axios'
export default {
  asyncData(context) {
    return axios
      .get(
        `https://nuxt-post-73233-default-rtdb.firebaseio.com/posts/${context.params.id}.json`
      )
      .then((res) => {
        return {
          loadedPosts: res.data,
        }
      })
      .catch((e) => console.log(context.error(e)))
  },
}
</script>

<style>
  
</style>