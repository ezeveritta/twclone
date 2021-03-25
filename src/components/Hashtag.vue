<template>

    <article class="border-top px-3 py-2">
        <div class="d-flex">

            <div class="w-100">
                <!-- [START] Usuario -->
                <span v-if="user != undefined" class="text-muted info usuario">
                    <b-link to="/">
                        <b-avatar class="avatar mr-2" />
                        <strong class="ff-bold" >{{user}}</strong>
                        <b-icon-patch-check-fill class="c-blue ml-1" />
                    </b-link>
                    <span> · {{date}}</span>
                </span>
                <!-- [START] Usuario -->

                <span class="text-muted why" v-if="why != ''">{{why}}</span>
                <div class="content"><strong>{{title}}</strong></div>

                <!-- [START] Información -->
                <span v-if="info != undefined" class="text-muted info">
                    {{info}}
                    <span v-if="this.info_links != undefined">
                        <b-link v-for="link of info_links" :key="link">{{link}} </b-link>
                    </span>
                </span>
                <!-- [END] Información -->
            </div>

            <div v-if="this.imagen != undefined">
                <b-img :src="imagen" alt="Imagen ilustrativa" />
            </div>
            <div v-else class="hashtag_menu">
                <b-icon-three-dots class="bgch-light-blue rounded-circle" scale=".45" />
            </div>

        </div>
    </article>
    
</template>

<script>
export default {
    name: 'Hashtag',
    props: {
        title: '',
        info: '',
        info_links: [],
        why: '',
        imagen: '',
        user: '',
        date: ''
    },
    methods: {
        
    }
}
</script>


<style scoped>

.hashtag_menu { position: relative; right: 10px; fill: gray;}
.hashtag_menu svg { font-size: 2rem; }

article { cursor: pointer; transition-duration: .1s; }
article:hover { background-color: #eee; }

img { width: 68px; height: 68px; border-radius: 10px; }

.why, .info { font-size: 14px; }

.usuario a:hover { text-decoration: none; }
.usuario .avatar { width: 18px; height: 18px; transform: translateY(-1px); }

</style>