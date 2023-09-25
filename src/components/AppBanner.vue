<script>
export default {
    name: 'AppBanner',

    data() {
        return {
            services: [
                {
                    img: 'buy-comics-digital-comics',
                    name: 'Digital comics'
                },
                {
                    img: 'buy-comics-merchandise',
                    name: 'dc merchandise'
                },
                {
                    img: 'buy-comics-subscriptions',
                    name: 'subscription'
                },
                {
                    img: 'buy-comics-shop-locator',
                    name: 'comic shop locator'
                },
                {
                    img: 'buy-dc-power-visa',
                    name: 'dc power visa'
                },
            ]

        }
    },

    methods: {
        getImageUrl(img) {
            return new URL(`./src/assets/${service.img}.png`, import.meta.url).href
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
                        <img :src="getImageUrl(img)" alt="">
                        <h5>
                            <a href="#" class="text-white text-decoration-none text-uppercase">
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