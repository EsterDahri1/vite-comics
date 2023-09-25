<script>
export default {
    name: 'AppComics',
    // props: ['thumb', 'price', 'series', 'type'],
    data() {
        return {
            // message: 'Hello AppComics'
        }
    }
}
</script>

<template>
    <div class="card">
        <!-- <h1>{{ message }}</h1> -->
        <img width="70"
            src="https://static.vecteezy.com/system/resources/previews/002/592/172/non_2x/smile-emoji-pop-art-line-style-icon-free-vector.jpg"
            alt="" class="img-card-top">
        <div class="card-body">
            Testo del fumetto
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;
</style>


<!-- <img :src="prop.thumb" class="card-img-top">
            <div class="card-body">
                <h4 class="text-muted text-uppercase text-white">{{ prop.series }}</h4>
            </div> -->