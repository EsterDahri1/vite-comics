<script>
export default {
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
            {{ message }}
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables';

.jumbotron {
    color: white;
    height: 130px;
}
</style>