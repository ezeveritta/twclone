<template>
    
    <header class="search w-100 pl-4 pr-5 py-1 bg-white">
        <div class="d-flex align-items-center rounded-pill">
        <b-icon-search />
        <b-input placeholder="Buscar en Twitter" />
        </div>
    </header>

</template>

<script>
export default {
    name: 'Buscador'
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