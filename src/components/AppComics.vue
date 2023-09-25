<script>
export default {
    name: 'AppComics',
    // props: ['thumb', 'price', 'series', 'type'],
    data() {
        return {
            message: 'Hello AppComics'
        }
    }
}
</script>

<template>
    <div>
        <h1>{{ message }}</h1>
    </div>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;
</style>


<!-- <img :src="prop.thumb" class="card-img-top">
            <div class="card-body">
                <h4 class="text-muted text-uppercase text-white">{{ prop.series }}</h4>
            </div> -->