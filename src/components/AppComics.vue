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
    <div class="col-2">
        <div class="card rounded-0 border-0">
            <!-- <h1>{{ message }}</h1> -->
            <img width='100' :src="thumb" alt="" class="img-card-top mt-4">
            <div class="card-body d-flex align-items-center justify-content-start p-0 pt-2">
                <h4 class="text-uppercase text-white">{{ series }}</h4>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

.card {
    background-color: transparent;

    img {
        width: 190px;
        aspect-ratio: 1 / 1;
        object-fit: cover;
    }

}
</style>

