<!--
Descrizione 1:
Create un nuovo progetto utilizzando Vite e Vue 3 e definite i componenti necessari per strutturare il layout come da screenshot allegato. ✔️

Quando la struttura a macroblocchi è pronta ✔️, popolate le voci di menu dinamicamente usando i data del componente. ✔️

Per oggi diamo priorità alla struttura: quando è tutto bello solido, passiamo al Sass! ✔️

Bonus:
Creare un componente aggiuntivo per gestire la fascia azzurra con le icone. ✔️

Descrizione 2:
create un nuovo componente che rappresenterà le card dei fumetti. ✔️
Utilizzate i dati presenti nel file json che trovate in allegato e passateli al componente Card tramite props. ✔️
-->

<script>
import AppHeader from './components/AppHeader.vue';
import AppJumbo from './components/AppJumbo.vue';
import AppBanner from './components/AppBanner.vue';
import AppFooter from './components/AppFooter.vue';

export default {
  data() {
    return {

    }
  },

  components: {
    AppHeader,
    AppJumbo,
    AppBanner,
    AppFooter
  }
}
</script>

<template>
  <AppHeader />
  <AppJumbo />
  <AppBanner />
  <AppFooter />
</template>

<style lang="scss">
@use'../src/assets/scss/app.scss'
</style>
