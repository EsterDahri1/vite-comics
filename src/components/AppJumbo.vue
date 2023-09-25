<script>
import comics from "../comics.js";
export default {
    name: 'AppJumbo',

    data() {
        return {
            comics
        }
    }
}
</script>

<template>
    <div class="teen pt-5 d-flex flex-column justify-content-end">
        <div class="bg-black">
            <div class="container jumbotron d-flex align-items-center justify-content-between">
                <div class="col-2 h-100">
                    <img :src="comics.thumb" class="card-img-top">
                    <div class="card-body">
                        <h4 class="text-muted text-uppercase text-white">{{ comics.series }}</h4>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
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