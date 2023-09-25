<script>
import comics from "../comics.js";
import AppComics from "./AppComics.vue";
export default {
    name: 'AppJumbo',


    components: {
        AppComics
    },

    data() {
        return {
            comics: comics
        }
    }
}
</script>

<template>
    <div class="teen d-flex flex-column justify-content-end">
        <div class="wrapper d-flex flex-column align-items-center justify-content-center">
            <div class="container jumbotron d-flex align-items-center justify-content-between flex-wrap">
                <div class="row pt-4 pb-1">
                    <AppComics v-for="comic in comics" :thumb="comic.thumb" :series="comic.series" />
                </div>
            </div>

            <a href="#" class="pe-5 ps-5 mb-3 mt-4 btn btn-primary rounded-0 text-uppercase fs-6">load more</a>
        </div>
    </div>
</template>

<style lang="scss">
@use '../assets/scss/partials/variables' as *;

.teen {
    height: 1000px;
    background-image: url(../assets/img/jumbotron.jpg);
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    object-fit: contain;

    .wrapper {
        background-color: $dc_dark;
    }
}

.jumbotron {
    color: white;
}
</style>