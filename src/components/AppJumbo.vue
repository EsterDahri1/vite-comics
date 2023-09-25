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
            comics
        }
    }
}
</script>

<template>
    <div class="teen d-flex flex-column justify-content-end">
        <div class="bg-black">
            <div class="container jumbotron d-flex align-items-center justify-content-between">
                <div class="row py-4">
                    <AppComics />
                </div>
                <!-- <div class="col-2 h-100" v-for="comic in comics">
                    <img :src="comic.thumb" class="card-img-top">
                    <div class="card-body">
                        <h4 class="text-muted text-uppercase text-white">{{ comic.series }}</h4>
                    </div>
                </div> -->
                <!-- :thumb="comic.thumb" :series="comic.series" v-for="comic in comics"  -->
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
    height: 500px;
}
</style>