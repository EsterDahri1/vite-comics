<script>
export default {
    data() {
        return {
            dcComicsLinks: ['Characters', 'Comics', 'Movies', 'TV', 'Games', 'Videos', 'News'],
            shopLinks: ['Shop DC', 'Shop DC Collectibles'],
            dcLinks: ['Terms Of Use', 'Privacy policy (New)', 'Ad Choices', 'Advertising', 'Jobs', 'Subscriptions', 'Talent Workshops', 'CPSC Certificates', 'Shop Help', 'Contact US'],
            sitesLinks: ['DC', 'MAD Magazine', 'DC Kids', 'DC Universe', 'DC Power Visa'],

            socials: [
                {
                    img: './src/assets/img/footer-facebook.png',
                    href: '##'
                },
                {
                    img: './src/assets/img/footer-twitter.png',
                    href: '##'
                },
                {
                    img: './src/assets/img/footer-youtube.png',
                    href: '##'
                },
                {
                    img: './src/assets/img/footer-pinterest.png',
                    href: '##'
                },
                {
                    img: './src/assets/img/footer-periscope.png',
                    href: '##'
                },
            ]
        }
    }
}
</script>

<template>
    <div id="upperFooter">
        <div class="container d-flex justify-content-between">
            <div class="col-4 d-flex flex-wrap mt-4">
                <div class="p-2">
                    <h4 class="text-uppercase text-white">dc comics</h4>
                    <ul class="list-unstyled p-0 fs-6">
                        <li v-for="dcComicsLink in dcComicsLinks">{{ dcComicsLink }}</li>
                    </ul>
                    <h4 class="text-uppercase text-white">shop</h4>
                    <ul class="list-unstyled p-0 fs-6">
                        <li v-for="shopLink in shopLinks">{{ shopLink }}</li>
                    </ul>
                </div>
                <div class="p-2">
                    <h4 class="text-uppercase text-white">dc</h4>
                    <ul class="list-unstyled p-0 fs-6">
                        <li v-for="dcLink in dcLinks">{{ dcLink }}</li>
                    </ul>
                </div>
                <div class="p-2">
                    <h4 class="text-uppercase text-white">sites</h4>
                    <ul class="list-unstyled p-0 fs-6">
                        <li v-for="sitesLink in sitesLinks">{{ sitesLink }}</li>
                    </ul>
                </div>
            </div>
            <img src="../assets/img/dc-logo-bg.png" alt="" srcset="" class="mb-4">
        </div>
    </div>
    <div id="lowerFooter" class="d-flex align-items-center">
        <div class="container d-flex justify-content-between align-items-center">
            <a href="#" class="btn btn-outline-primary text-uppercase text-white rounded-0 fs-4 border-3">sign-up now!</a>
            <div class="social d-flex align-items-center justify-content-center">
                <h4 class="text-uppercase text-primary p-2 pt-2 m-0 text-center">follow us</h4>
                <img v-for="social in socials" :src="social.img" class="text-white p-1" alt="">
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use'../assets/scss/partials/variables' as *;

#upperFooter {
    height: 400px;
    background-image: url(../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    overflow-y: hidden;

    li {
        color: rgba(255, 255, 255, 0.57)
    }
}

;

#lowerFooter {
    height: 100px;
    background-color: $dc_dark;

}
</style>