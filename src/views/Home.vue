<template>

  <b-row class="v-home"  no-gutters>
    
    <!-- Posts -->
    <b-col class="home-content border-right">

      <!-- Preferencia de contenido -->
      <HomeFilter />

      <!-- Nuevo Post -->
      <NewPost />

      <!-- Post List -->
      <div class="Post-list mt-3 bg-white">
        hola
      </div>

    </b-col>

    <!-- Recomendaciones -->
    <b-col cols="5">

      <!-- Buscador -->
      <div class="search">
        <input type="text">
      </div>

      <!-- Explorar -->
      <div>
        hola
      </div>

    </b-col>

  </b-row>

</template>

<script>
// @ is an alias to /src
import HomeFilter from '@/components/HomeFilter.vue'
import NewPost from '@/components/NewPost.vue'

export default {
  name: 'Home',
  components: {
    HomeFilter, NewPost
  }
}
</script>


<style scoped>

.home-content { background-color: #eee; }

</style>