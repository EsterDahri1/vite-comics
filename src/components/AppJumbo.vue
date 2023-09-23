<script>
export default {
    name: 'AppJumbo',

    data() {
        return {
            message: '--> Content goes here <--'
        }
    }
}
</script>

<template>
    <div class="bg-black">
        <div class="container jumbotron d-flex justify-content-start align-items-center">
            <h2>{{ message }}</h2>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

.jumbotron {
    color: $dc_light;
    height: 130px;
}
</style>