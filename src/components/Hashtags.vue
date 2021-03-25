<template>

    <section class="Hashtags pl-4 pr-5 py-1 mt-3">
        <div class="">
            <header class="pt-3 pb-2 px-3">
                <h5 class="ff-bold">¿Qué está pasando?</h5>
            </header>

            <Hashtag title="Toy Story" why="Política - Tendencia" 
                     info='Tendencias sobre ' :info_links="['Cristina,', 'Maléfica']" />

            <Hashtag title="Perez" info="6245 Tweets" why="Tendencia en Twitter" imagen="https://pbs.twimg.com/media/ExLruCIVcBUb5Zn?format=jpg" />

            <Hashtag title="Feliz cumpleaños Elton John" why="Música - EN DIRECTO" imagen="https://pbs.twimg.com/semantic_core_img/1371898551274336257/9F5ZFqVR?format=jpg&name=240x240" />

            <Hashtag title="Scarlett" info="16,7 mil Tweets" why="Tendencia en Argentina" />

            <Hashtag title="TODOS los estrenos de Netflix para abril 2021" imagen="https://pbs.twimg.com/media/ExRFy7VWUAEK9X6?format=jpg&name=120x120"
                     user="GQ México y Latam" date="Ayer" />

            <footer class="w-100 border-top">
                <b-link class="d-block px-3 py-3">
                    Mostrar más
                </b-link>
            </footer>
        </div>
    </section>
    
</template>

<script>
import Hashtag from '@/components/Hashtag.vue'

export default {
    name: 'Hashtags',
    components: {
        Hashtag
    },
    methods: {
        Hashtag_links(links) {
            return links;
        }
    }
}
</script>


<style scoped>

.Hashtags > div { background-color: rgb(245, 245, 245); border-radius: 15px; }

.Hashtags > div > footer:hover { background-color: #eee; border-radius: 15px; }
.Hashtags > div > footer:hover a { text-decoration: none!important; }

</style>