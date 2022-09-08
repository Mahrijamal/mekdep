<template>
  <div class="admin_page">
    <div class="new_post">
      <nuxt-link to="/admin/new_post" class="new_btn">Create Post</nuxt-link>
    </div>
    <div class="cards">
        <Card i v-for="(e, i) in products" :key="i" :info="e" :isAdmin="true" />
    </div>
  </div>
</template>

<script>
import Card from '@/components/card.vue'
export default {
  components: {
    Card,
  },
  computed:{
    products(){
        return this.$store.getters.products12;
    }
  }
}
</script>

<style scoped>
.new_post{
    display: flex;
    align-items: center;
    justify-content: center;
    margin-top: 30px;
}
.new_btn{
    padding: 10px 30px;
    display: block;
    background: lightgreen;
    border-radius: 20px;
    text-decoration: none;
}
.cards{
  width: 300px;
}
</style>