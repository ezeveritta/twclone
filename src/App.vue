<template>

  <!--
    El sitio se divide en 2 partes:
    - La primera es la columna que contiene la barra de navegación estática tanto en el sitio como en la posición de la página.
    - La segunda es la columna donde se muestran las vistas de cada página.
  -->
  <b-container class="" style="max-width: 100%!important;">
    <b-row id="app" no-gutters>

      <!-- Sidebar - Navbar -->
      <b-col cols="3" style="max-width: 313px">
        <aside class="">
          <Navbar id="navbar"/>
        </aside>
      </b-col>

      <!-- View - Content -->
      <b-col>
        <main class="border-left">
          <router-view />
        </main>
      </b-col>
      
    </b-row>
  </b-container>
  
</template>

<script>
import Navbar from '@/components/Navbar.vue'

export default {
  name: 'App',
  components: {
    Navbar
  }
}
</script>

<style>

/********************************************************************************************************
 * FUENTE Segoe UI
 */
@font-face {
font-family: 'segoeUI';
font-style: normal;
font-weight: normal;
src: local('assets/fonts/Segoe UI Regular'), url('assets/fonts/Segoe UI.woff') format('woff');
}


@font-face {
font-family: 'segoeUI-italic';
font-style: italic;
font-weight: normal;
src: local('assets/fonts/Segoe UI Italic'), url('assets/fonts/Segoe UI Italic.woff') format('woff');
}


@font-face {
font-family: 'segoeUI-bold';
font-style: normal;
font-weight: bold;
src: local('assets/fonts/Segoe UI Bold'), url('assets/fonts/Segoe UI Bold.woff') format('woff');
}


@font-face {
font-family: 'segoeUI-bold-italic';
font-style: italic;
font-weight: bold;
src: local('assets/fonts/Segoe UI Bold Italic'), url('assets/fonts/Segoe UI Bold Italic.woff') format('woff');
}

* { font-family: 'segoeUI'!important; }
.ff-italic { font-family: 'segoeUI-italic'!important; }
.ff-bold { font-family: 'segoeUI-bold'!important; }
.ff-bold-italic { font-family: 'segoeUI-bold-italic'!important; }


/********************************************************************************************************
 * COLORES
 */

* { color: #14171A }

/* Color de texto */
.c-blue { color: #1DA1F2!important; fill: #1DA1F2!important }
.c-light-blue { color: rgba(29, 161, 242, 0.1); fill: rgba(29, 161, 242, 0.1) }
.c-black { color: #14171A!important; fill: #14171A!important }
.c-dark-gray { color: #657786!important; fill: #657786!important }
.c-light-gray { color: #AAB8C2!important; fill: #AAB8C2!important }
.c-extra-light-gray { color: #E1E8ED!important; fill: #E1E8ED!important }
.c-white { color: #F5F8FA!important; fill: #F5F8FA!important }

/* Color de texto en :hover */
.ch-blue:hover { color: #1DA1F2!important; fill: #1DA1F2!important }
.ch-light-blue:hover { color: rgba(29, 161, 242, 0.1); fill: rgba(29, 161, 242, 0.1) }
.ch-black:hover { color: #14171A!important; fill: #14171A!important }
.ch-dark-gray:hover { color: #657786!important; fill: #657786!important }
.ch-light-gray:hover { color: #AAB8C2!important; fill: #AAB8C2!important }
.ch-extra-light-gray:hover { color: #E1E8ED!important; fill: #E1E8ED!important }
.ch-white:hover { color: #F5F8FA!important; fill: #F5F8FA!important }

/* Color de fondo */
.bgc-blue { background-color: #1DA1F2!important }
.bgc-light-blue { background-color: rgba(29, 161, 242, 0.1) }
.bgc-black { background-color: #14171A!important }
.bgc-dark-gray { background-color: #657786!important }
.bgc-light-gray { background-color: #AAB8C2!important }
.bgc-extra-light-gray { background-color: #E1E8ED!important }
.bgc-white { background-color: #F5F8FA!important }

/* Color de fondo en :hover */
.bgch-blue:hover { background-color: #1DA1F2!important }
.bgch-dark-blue:hover { background-color: #128bd6!important }
.bgch-light-blue:hover { background-color: rgba(29, 161, 242, 0.1) }
.bgch-light-green:hover { background-color: rgba(23, 191, 99, 0.1) }
.bgch-black:hover { background-color: #14171A!important }
.bgch-dark-gray:hover { background-color: #657786!important }
.bgch-light-gray:hover { background-color: #AAB8C2!important }
.bgch-extra-light-gray:hover { background-color: #E1E8ED!important }
.bgch-white:hover { background-color: #F5F8FA!important }


button:focus, button:active, button:hover
input:focus, input:active, input:hover { box-shadow: none!important; outline: none!important; }

/********************************************************************************************************
 * NAVBAR's POPOVER
 */
.popover { overflow: hidden; border-radius: 18px!important; }
.popover-body { padding: 0px!important }
.popover * { border: none!important }


.menu { position: fixed!important; height: 100%; width: 275px; left: 44px;}

</style>