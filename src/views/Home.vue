<template>
  <b-row class="v-home"  no-gutters>
    
    <!-- Posts -->
    <b-col class="home-content border-right">

      <!-- Preferencia de contenido -->
      <HomeFilter />

      <!-- Nuevo Post -->
      <NewPost />
      
      <div class="d-block w-100" style="height: 12px; background-color: #EEEEEE"></div>

      <!-- Post List -->
      <section class="Post-list px-3">

        Lorem ipsum dolor sit amet consectetur adipisicing elit. Illum at possimus quidem, 
        esse molestias temporibus recusandae beatae laboriosam magnam impedit, architecto ea, laborum quasi. 
        Quo consequatur optio inventore eligendi laboriosam!
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Illum at possimus quidem, 
        esse molestias temporibus recusandae beatae laboriosam magnam impedit, architecto ea, laborum quasi. 
        Quo consequatur optio inventore eligendi laboriosam!
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Illum at possimus quidem, 
        esse molestias temporibus recusandae beatae laboriosam magnam impedit, architecto ea, laborum quasi. 
        Quo consequatur optio inventore eligendi laboriosam!
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Illum at possimus quidem, 
        esse molestias temporibus recusandae beatae laboriosam magnam impedit, architecto ea, laborum quasi. 
        Quo consequatur optio inventore eligendi laboriosam!
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Illum at possimus quidem, 
        esse molestias temporibus recusandae beatae laboriosam magnam impedit, architecto ea, laborum quasi. 
        Quo consequatur optio inventore eligendi laboriosam!
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Illum at possimus quidem, 
        esse molestias temporibus recusandae beatae laboriosam magnam impedit, architecto ea, laborum quasi. 
        Quo consequatur optio inventore eligendi laboriosam!
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Illum at possimus quidem, 
        esse molestias temporibus recusandae beatae laboriosam magnam impedit, architecto ea, laborum quasi. 
        Quo consequatur optio inventore eligendi laboriosam!
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Illum at possimus quidem, 
        esse molestias temporibus recusandae beatae laboriosam magnam impedit, architecto ea, laborum quasi. 
        Quo consequatur optio inventore eligendi laboriosam!
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Illum at possimus quidem, 
        esse molestias temporibus recusandae beatae laboriosam magnam impedit, architecto ea, laborum quasi. 
        Quo consequatur optio inventore eligendi laboriosam!
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Illum at possimus quidem, 
        esse molestias temporibus recusandae beatae laboriosam magnam impedit, architecto ea, laborum quasi. 
        Quo consequatur optio inventore eligendi laboriosam!
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Illum at possimus quidem, 
        esse molestias temporibus recusandae beatae laboriosam magnam impedit, architecto ea, laborum quasi. 
        Quo consequatur optio inventore eligendi laboriosam!

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
import NewPost from '@/components/NewPost.vue'

export default {
  name: 'Home',
  components: {
    HomeFilter, NewPost
  }
}
</script>


<style scoped>

.home-content {  }

.search {z-index: 1; position: -webkit-sticky; position: sticky; top: 0px; background: #ccc; }
.search > div { padding: 5px; background: #EEE; }
.search input { background-color: transparent!important; border: none;  }
.search svg { margin-left: 14px; margin-top: 2px; fill: gray; }

.search > div:hover { padding: 5px; background: #EEE; }
.search > div:focus-within { box-shadow: 0 0 0 1px #1DA1F2; background: transparent; }
.search > div:focus-within svg { fill: #1DA1F2; }
</style>