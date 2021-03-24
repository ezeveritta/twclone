<template>
    <div class="d-flex px-3 py-2 border-bottom">

        <b-avatar class="avatar"></b-avatar>

        <div class="w-100 ml-3">

            <div class="text mt-2">
                <div class="w-100 h-auto" role="textarea" aria-multiline="true" contenteditable="true">
                    <a href="/asda">#asdasd</a> asdasd
                </div>
            </div>

            <div class="Permitidos border-bottom pb-3 mt-3">
                <b-button class="bgch-light-blue rounded-pill p-0" size="sm" variant="link">
                    <b-icon-slack scale="0.9" class="c-blue" />
                    <span class="ml-2 c-blue ff-bold mr-2">Cualquier persona puede responder</span>
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

.avatar { width: 48px; height: 48px }

.text > div { outline: none; user-select: text; white-space: pre-wrap; overflow-wrap: break-word; font-size: 20px; }
.text a { color: #1DA1F2; }

.Permitidos { margin-top: -4px }

.media-buttons { margin-top: -13px; margin-left: -12px }
.media-buttons > button { width: 28px; height: 28px; margin-right: 15px; font-size: 1.8rem }

.send-tweet > * { margin-left: 15px }

.send-tweet .add { width: 22px; height: 22px; font-size: 1.5rem; margin-top: -32px; margin-right: 15px }
.send-tweet .add svg { border: 1px solid #1DA1F2;  }

</style>