<template>
    <div class="HomeFilter border-bottom bg-white">

        <div class="d-flex justify-content-between px-3 py-2">
            <div class="filter-name ff-bold">
                Inicio
            </div>
            <div class="filter-button bgch-light rounded-circle">
                <b-icon-search />
            </div>
        </div>

    </div>
</template>

<script>

export default ({
    name: 'HomeFilter'
})
</script>


<style scoped>

.HomeFilter { position: relative; width: 100%; cursor: pointer }

</style>