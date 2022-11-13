<template>
  <div id="app">
    <HeaderGamesOn />
    <HomeGameOn />
    <CardGamesOn />
    <FooterGameOn />
  </div>
</template>

<script>
import './styles/global.css';
import HeaderGamesOn from './components/HeaderGamesOn.vue';
import HomeGameOn from './pages/HomeGameOn.vue';
import CardGamesOn from './components/CardsGamesOn.vue'
import FooterGameOn from './components/FooterGameOn.vue';
export default {
  name: 'App',
  components: {
    HeaderGamesOn,
    HomeGameOn,
    FooterGameOn,
    CardGamesOn
}
}
</script>

<style lang="scss">

</style>
