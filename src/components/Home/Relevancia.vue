<template>
    <div class="Relevancia border-bottom bg-white">

        <div class="d-flex justify-content-between p-3">

            <header class="filter-name ff-bold h5 mb-0">
                Tweets más recientes
            </header>

            <div class="filter-button bgch-light rounded-circle">
                <b-icon-search />
            </div>
        </div>

    </div>
</template>

<script>

export default ({
    name: 'Relevancia'
})
</script>


<style>

.Relevancia { width: 100%; cursor: pointer; z-index: 1;  position: -webkit-sticky; position: sticky; top: 0px; }

</style>