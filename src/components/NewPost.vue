<template>
    <div class="d-flex bg-white p-2">

        <b-avatar></b-avatar>

        <div class="w-100 ml-2">

            <div class="text">
                <textarea class="w-100" placeholder="¿Qué está pasando?"></textarea>
            </div>

            <div class="region border-bottom">
                <b-button class="bgch-light-blue rounded-pill p-0 px-2 py-1" variant="link">
                    <b-icon-search scale="0.65" class="c-blue" />
                    <small class="ml-1 c-blue">Cualquier persona puede responder</small>
                </b-button>
            </div>

            <div class="media">
                <div class="d-flex justify-content-between align-center">
                    <div class="media-buttons">
                        <b-button>
                            <b-icon-search></b-icon-search>
                        </b-button>

                        <b-button>
                            <b-icon-search></b-icon-search>
                        </b-button>

                        <b-button>
                            <b-icon-search></b-icon-search>
                        </b-button>

                        <b-button>
                            <b-icon-search></b-icon-search>
                        </b-button>

                        <b-button>
                            <b-icon-search></b-icon-search>
                        </b-button>
                    </div>
                    <div class="send-tweet">
                        <button>Twittear</button>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>