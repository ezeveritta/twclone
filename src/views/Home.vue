<template>
  <b-row class="v-home"  no-gutters>
    
    <!-- Tweets -->
    <b-col class="home-content border-right">

      <!-- Preferencia de contenido -->
      <HomeFilter />

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
        <div class="search w-100 pl-4 pr-5 py-1 bg-white">
          <div class="d-flex align-items-center rounded-pill">
            <b-icon-search />
            <b-input placeholder="Buscar en Twitter" />
          </div>
        </div>

        <!-- Explorar -->
        <section>

          hola

        </section>

      </aside>
    </b-col>
  </b-row>
</template>

<script>
// @ is an alias to /src
import HomeFilter from '@/components/HomeFilter.vue'
import NewTweet from '@/components/NewTweet.vue'
import Tweet from '@/components/Tweet.vue'

export default {
  name: 'Home',
  components: {
    HomeFilter, NewTweet, Tweet
  }
}
</script>


<style scoped>


.search {z-index: 1; position: -webkit-sticky; position: sticky; top: 0px; background: #ccc; }
.search > div { padding: 5px; background: #EEE; }
.search input { background-color: transparent!important; border: none;  }
.search svg { margin-left: 14px; margin-top: 2px; fill: gray; }

.search > div:hover { padding: 5px; background: #EEE; }
.search > div:focus-within { box-shadow: 0 0 0 1px #1DA1F2; background: transparent; }
.search > div:focus-within svg { fill: #1DA1F2; }
</style>