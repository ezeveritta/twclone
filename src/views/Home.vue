<template>
  <b-row class="v-home"  no-gutters>
    
    <!-- Tweets -->
    <b-col class="home-content border-right">

      <!-- Preferencia de contenido -->
      <Relevancia />

      <!-- Nuevo Tweet -->
      <NewTweet />
      
      <div class="d-block w-100" style="height: 12px; background-color: #EEEEEE"></div>

      <!-- Tweet List -->
      <section class="Tweet-list">
        
        <Tweet />
        
        <Tweet />

      </section>

    </b-col>

    <!-- Recomendaciones -->
    <b-col cols="5" class="h-100">
      <aside>

        <!-- Buscador -->
        <Buscador />

        <!-- Explorar -->
        <section>

          <Hashtags />

        </section>

      </aside>
    </b-col>
  </b-row>
</template>

<script>
// @ is an alias to /src
import Relevancia from '@/components/Home/Relevancia.vue'
import NewTweet from '@/components/Home/NewTweet.vue'
import Buscador from '@/components/Home/Buscador.vue'
import Tweet from '@/components/Tweet.vue'
import Hashtags from '@/components/Hashtags.vue'

export default {
  name: 'Home',
  components: {
    Relevancia, NewTweet, Tweet, Hashtags, Buscador
  }
}
</script>


<style scoped>

</style>