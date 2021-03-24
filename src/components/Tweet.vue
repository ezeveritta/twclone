<template>
    <article class="Tweet border-top px-3 pt-3 pb-2">

        <div class="position-absolute Tweet-option">
            <b-icon-three-dots scale="0.5" class="bgch-light-blue rounded-circle" />
        </div>

        <div class="d-flex w-100">

            <b-avatar class="avatar mr-3" />

            <div>
                <header>
                    <b-link to="/">
                        <strong class="ff-bold" >Formula 1 </strong>
                        <b-icon-patch-check-fill class="c-blue" />
                        <span class="text-muted"> @F1</span>
                    </b-link>
                    <span> · </span>
                    <b-link to="/" class="text-muted">
                        1h
                    </b-link>
                </header>

                <section class="content">

                    Coming out fighting! 
                    <span role="img" title="Guante de Boxeo">🥊</span>
                    <br>
                    <a href="#">#BahrainGP</a> 
                    <span title="Bandera de Baréin">🇧🇭</span> <a href="#">#F1</a> 

                </section>

                <section class="embed mt-2 border">
                    <div>
                        <b-img class="w-100" src="https://pbs.twimg.com/card_img/1374732400001871881/V50AUG0c?format=jpg&name=small" />
                        <article class="p-3">
                            <header>'I'm botter' than the likes of hamilton, Verstappen and Vettel, says ...</header>
                            <section>
                                <p class="text-muted">
                                    Returning tho-time champion Fernando Alonso isn't sure how
                                    Alpine will fare in 2021, but he is sure of his own talent as he ...
                                </p>
                                <b-icon-link scale="1.3" style="fill: gray" /><span class="text-muted ml-2">formula1.com</span>
                            </section>
                        </article>
                    </div>
                </section>

                <footer class="mt-2">
                    <b-row>
                        <!-- Comentarios -->
                        <b-col  class="text-muted comentarios d-flex align-items-center">
                            <b-icon-chat scale="0.5" class="rounded-circle mr-2" />
                            <span class="text-muted">368</span>
                        </b-col>

                        <!-- Retweets -->
                        <b-col  class="text-muted retweets d-flex align-items-center">
                            <b-icon-arrow-repeat scale="0.5" class="rounded-circle mr-2" />
                            <span class="text-muted">368</span>
                        </b-col>

                        <!-- Likes -->
                        <b-col  class="text-muted likes d-flex align-items-center">
                            <b-icon-heart scale="0.5" class="rounded-circle mr-2" />
                            <span class="text-muted">368</span>
                        </b-col>

                        <!-- Compartir -->
                        <b-col  class="text-muted compartir d-flex align-items-center">
                            <b-icon-upload scale="0.5" class="rounded-circle mr-2" />
                        </b-col>

                    </b-row>
                </footer>
            </div>

        </div>

    </article>
</template>

<script>
export default {
    name: 'Tweet',
    props: {
        user: { name: 'name', username: 'username', avatar: 'avatar'},
        info: { date: '01-03-2021 12:48:22', comments: 0, retweets: 1, likes: 2 },
        content: { 
            id: '1',
            text: "Texto de Prueba",
            media: { image: '', video: '', link: '' }
        }
    }
}
</script>

<style>

.Tweet { cursor: pointer; transition-duration: .2s; }
.Tweet:hover { background-color: #f5f5f5; }

.Tweet .Tweet-option { right: 15px; font-size: 2.4rem; fill: gray; transform: translateY(-18px); }

.Tweet .avatar { width: 48px!important; height: 48px!important; }

.Tweet .embed { border-radius: 16px; overflow: hidden; }
.Tweet .embed { font-size: 14px; }

/** Botones */
.Tweet footer svg { fill: gray; }
.Tweet footer { }

/** Hovers */
.Tweet footer svg { font-size: 2.1rem; }

.Tweet .comentarios:hover span { color: #1DA1F2!important; }
.Tweet .comentarios:hover svg { fill: #1DA1F2; background-color: rgba(29, 161, 242, 0.1); }

.Tweet .retweets:hover span { color: rgba(23, 191, 99, 1)!important; }
.Tweet .retweets:hover svg { fill: rgba(23, 191, 99, 1); background-color: rgba(23, 191, 99, 0.1); }

.Tweet .likes:hover span { color: rgba(224, 36, 94, 1)!important; }
.Tweet .likes:hover svg { fill: rgba(224, 36, 94, 1); background-color: rgba(224, 36, 94, 0.1); }

.Tweet .compartir:hover svg { fill: #1DA1F2; background-color: rgba(29, 161, 242, 0.1); }

</style>