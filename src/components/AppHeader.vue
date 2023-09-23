<script>
import AppLogo from './AppLogo.vue';
export default {
    name: 'AppHeader',
    data() {
        return {
            navBarItems: ['characters', 'comics', 'movies', 'tv', 'games', 'collectibles', 'videos', 'fans', 'news', 'shop'],

            activeLink: 0
        }
    },

    components: {
        AppLogo
    }
}
</script>

<template>
    <header class="mt-1 d-flex justify-content-between align-items-center container">
        <AppLogo />

        <div>
            <nav class="p-0 navbar navbar-expand navbar-light">
                <ul class="nav nav-bar-nav" v-for="(item, index) in navBarItems">
                    <li class="nav-item" @click="activeLink = index">
                        <a href="#" class="nav-link" :class="activeLink === index ? 'active' : ''">{{ item
                        }}</a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<style lang='scss' scoped>
@use '../assets/scss/partials/variables' as *;

header {
    height: 120px;

    li {
        a {
            text-transform: uppercase;
            color: $dc_dark;

            &.active {
                color: $dc_primary;
            }
        }

        & a.active {
            color: $dc_primary;
            border-bottom: solid 5px $dc_primary;
        }
    }
}
</style>