<script>
export default {
    name: 'AppComics',
    props: {
        thumb: String,
        price: String,
        series: String,
        type: String,
    },
    data() {
        return {
            // message: 'Hello AppComics'
        }
    }
}
</script>

<template>
    <div class="card rounded-0">
        <!-- <h1>{{ message }}</h1> -->
        <img :src="thumb" alt="" class="img-card-top">
        <div class="card-body">
            <h4 class="text-uppercase text-white">{{ series }}</h4>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

.card {
    background-color: transparent;

}
</style>


<!-- <img :src="prop.thumb" class="card-img-top">
            <div class="card-body">
                <h4 class="text-muted text-uppercase text-white">{{ prop.series }}</h4>
            </div> -->