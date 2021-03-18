<template>
    <!--
        El Navbar permanece en posición estática y es una lista en vertical de botones de variados estílos.
        Hay 4 cambios de estilos principales:
            - Ordenador: en un display amplio, los botones se muestran con un icono y el texto.
            - Tablet:    en un display mediano, los botones se muestran únicamente con los íconos.
            - Movil:     en un display pequeño, solo se muestran 4 botones y en un navbar horizontal en la
                         parte inferior de la pantalla.
            - Height:    cambiar el tamaño del display en forma vertical, oculta algunos botones.
    -->
    <b-navbar class="navbar">
        
        <div to="/"  class="twitter-icon active-link">
            <div class="btn rounded-circle" >
                <b-icon-twitter class="c-blue twitter-svg" />
            </div>
        </div>
        
        <b-list-group class="list  mt-3">

            <b-list-group-item to="/" active-class="active-link">
                <div class="btn rounded-pill">
                    <b-icon-house-door-fill />
                    Inicio
                </div>
            </b-list-group-item>

            <b-list-group-item to="/explorar">
                <div class="btn rounded-pill">
                    <b-icon-hash />
                    Explorar
                </div>
            </b-list-group-item>

            <b-list-group-item to="/notificaciones">
                <div class="btn rounded-pill">
                    <b-icon-bell />
                    Notificaciones
                </div>
            </b-list-group-item>

            <b-list-group-item to="/mensajes">
                <div class="btn rounded-pill">
                    <b-icon-chat-dots />
                    Mensajes
                </div>
            </b-list-group-item>

            <b-list-group-item to="/guardados">
                <div class="btn rounded-pill">
                    <b-icon-bookmark />
                    Guardados
                </div>
            </b-list-group-item>

            <b-list-group-item to="/listas">
                <div class="btn rounded-pill">
                    <b-icon-card-text />
                    Listas
                </div>
            </b-list-group-item>

            <b-list-group-item to="/perfil">
                <div class="btn rounded-pill">
                    <b-icon-person />
                    Perfil
                </div>
            </b-list-group-item>

            <b-list-group-item to="/">
                <div class="btn rounded-pill">
                    <b-icon-three-dots />
                    Más opciones
                </div>
            </b-list-group-item>

        </b-list-group>
        
        
        <div class="mt-3">
            <b-button size="lg" class="w-100 bgc-blue p-2 rounded-pill button-simple">Twittear</b-button>
        </div>

        <!-- 
            Botón para elegir el usuario.
        -->
        <b-button class="me d-flex justify-content-between rounded-pill p-2" id="popover-target-1">
            <ProfileSimple name="Ezequiel Vera" username="ezeveritta" avatar="https://pbs.twimg.com/profile_images/1363201646218665985/UlCcC7tE_200x200.jpg" />
            <b-icon-three-dots />

            <b-popover target="popover-target-1" triggers="focus" placement="top">

                <div class="d-flex justify-content-between p-3">
                    <ProfileSimple name="Ezequiel Vera" username="ezeveritta" avatar="https://pbs.twimg.com/profile_images/1363201646218665985/UlCcC7tE_200x200.jpg" />
                    <b-icon-check2 class="mt-2 c-blue" />
                </div>

                <b-list-group>
                    
                    <b-list-group-item to="/" class="border-top px-4">
                        Agregar una cuenta Existente
                    </b-list-group-item>

                    <b-list-group-item to="/" class="border-top px-4">
                        Cerrar la sesion de @ezeveritta
                    </b-list-group-item>

                </b-list-group>
            </b-popover>
        </b-button>
    </b-navbar>
</template>

<script>
import ProfileSimple from '@/components/ProfileSimple.vue'

export default {
    name: 'Navbar',
    components: { ProfileSimple }
}
</script>

<style scoped>

.navbar { display: block; width: 100%; height: 100vh; }
.navbar * { border: none; }

.twitter-icon div:hover { background: rgba(29, 161, 242, 0.1)!important }

.navbar .list > * { margin-top: -10px; }
.navbar .list div { font-size: 18px; font-family: 'segoeUI-bold'!important }
.navbar .list a { padding: 4px 16px 14px 3px!important; }
.navbar .list a:hover { background: transparent; }
.navbar .list a:hover * { color: #1DA1F2!important; fill: #1DA1F2; }
.navbar .list a:hover div { background: rgba(29, 161, 242, 0.1)!important }
.navbar svg:not(.twitter-svg) { margin-right: 10px;}

.navbar .me { position: absolute; bottom: 8px; cursor: pointer; width: 90%; background: transparent; }
.navbar .me:hover { background: rgba(29, 161, 242, 0.1);; }
.navbar .me:focus { background: rgba(29, 161, 242, 0.2)!important;; }
.navbar .me svg { font-size: 1.2rem; margin-top: 8px; }

button:focus, button:active, button:hover { box-shadow: none!important; outline: none!important;; }

.active-link * { color: #1DA1F2; fill: #1DA1F2; }


</style>