<script>
export default {
    name: 'AppBanner',

    data() {
        return {
            services: [
                {
                    img: '../assets/img/buy-comics-digital-comics.png',
                    name: 'Digital comics'
                },
                {
                    img: '../assets/img/buy-comics-merchandise.png',
                    name: 'dc merchandise'
                },
                {
                    img: '../assets/img/buy-comics-subscriptions.png',
                    name: 'subscription'
                },
                {
                    img: '../assets/img/buy-comics-shop-locator.png',
                    name: 'comic shop locator'
                },
                {
                    img: '../assets/img/buy-dc-power-visa.svg',
                    name: 'dc power visa'
                },
            ]

        }
    }
}
</script>

<template>
    <div class="banner d-flex align-items-center">
        <div class="container">
            <div class="row align-items-center justify-content-center">
                <div class="col-2" v-for="service in services">
                    <div class="d-flex align-items-center">
                        <img :src="service.img" alt="">
                        <h5>
                            <a href="#" class="text-white text-decoration-none">
                                {{ service.name }}
                            </a>
                        </h5>
                    </div>
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
    color: white;

    .col-2 {
        width: calc(100% / 10 * 2);
    }
}
</style>