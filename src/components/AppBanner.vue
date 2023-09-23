<script>
export default {
    name: 'AppBanner',

    data() {
        return {


        }
    }
}
</script>

<template>
    <div class="banner">
        <div class="row">
            <div class="col-2">
                <div>

                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use'../assets/scss/partials/variables' as *;

.banner {
    background-color: $dc_primary;
    height: 150px;
    color: $dc_light;

    .col-2 {
        width: calc(100% / 10 * 2);
    }
}
</style>