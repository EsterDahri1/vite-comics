<script>
export default {
    name: 'AppComics',
    props: {
        thumb: String,
        price: String,
        series: String,
        type: String,
    },
}
</script>

<template>
    <div class="col-2 h-100" v-for="comic in comics">
        <div class="card">
            <img :src="thumb" class="card-img-top">
            <div class="card-body">
                <h4 class="text-muted text-uppercase text-white">{{ series }}</h4>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;
</style>