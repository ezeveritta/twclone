<template>
    <div class="d-flex bg-white p-2">

        <b-avatar></b-avatar>

        <div class="w-100 ml-2">

            <div class="text">
                <div class="w-100 h-auto" role="textarea" aria-multiline="true" contenteditable="true" style="outline: none; user-select: text; white-space: pre-wrap; overflow-wrap: break-word;">
                    <a href="/asda"> asdasd </a>
                </div>
                <!-- TextArea antiguo, mientras pruebo un contenedor con contenteditable
                <textarea class="w-100 border-0" style="height: 35px; rezisable: none" placeholder="¿Qué está pasando?">
                    <a href="/asda"> asdasd </a>
                </textarea>
                -->
            </div>

            <div class="Permitidos border-bottom pb-2">
                <b-button class="bgch-light-blue rounded-pill p-0" size="sm" variant="link">
                    <b-icon-search scale="0.6" class="c-blue" />
                    <small><small class="ml-1 c-blue ff-bold mr-2">Cualquier persona puede responder</small></small>
                </b-button>
            </div>

            <div class="media mt-2 w-100">
                <div class="d-flex justify-content-between w-100">

                    <div class="media-buttons text-center">
                        <b-button variant="link">
                            <b-icon-image scale="0.5" class="bgch-light-blue c-blue rounded-circle" />
                        </b-button>

                        <b-button variant="link">
                            <b-icon-badge4k scale="0.5" class="bgch-light-blue c-blue rounded-circle" />
                        </b-button>

                        <b-button variant="link">
                            <b-icon-bar-chart-line rotate="90" scale="0.5" class="bgch-light-blue c-blue rounded-circle" />
                        </b-button>

                        <b-button variant="link">
                            <b-icon-emoji-smile scale="0.5" class="bgch-light-blue c-blue rounded-circle" />
                        </b-button>

                        <b-button variant="link">
                            <b-icon-calendar2-event scale="0.5" class="bgch-light-blue c-blue rounded-circle" />
                        </b-button>
                    </div>

                    <div class="send-tweet">

                        <span> | </span>

                        <b-button variant="link" class="add">
                            <b-icon-plus scale="0.8" class="bgch-light-blue c-blue rounded-circle" />
                        </b-button>

                        <button variant="link" class="bgch-dark-blue bgc-blue text-white rounded-pill border-0 py-1 px-3">Twittear</button>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>


<style scoped>

.Permitidos { margin-top: -4px }

.media-buttons { margin-top: -13px; margin-left: -12px }
.media-buttons > button { width: 28px; height: 28px; margin-right: 15px; font-size: 1.8rem }

.send-tweet > * { margin-left: 15px }

.send-tweet .add { width: 22px; height: 22px; font-size: 1.5rem; margin-top: -32px; margin-right: 15px }
.send-tweet .add svg { border: 1px solid #1DA1F2;  }

</style>