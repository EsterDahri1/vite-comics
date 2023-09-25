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
        <div class="bg-black">
            <div class="container jumbotron d-flex align-items-center justify-content-between flex-wrap">
                <div class="row py-4">
                    <AppComics v-for="comic in comics" :thumb="comic.thumb" :series="comic.series" />
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss">
@use '../assets/scss/partials/variables' as *;

.teen {
    height: 800px;
    background-image: url(../assets/img/jumbotron.jpg);
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
}

.jumbotron {
    color: white;
}
</style>