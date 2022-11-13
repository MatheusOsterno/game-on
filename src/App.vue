<template>
  <div id="app">
    <HeaderGamesOn />
    <HomeGameOn />
    <FooterGameOn />
  </div>
</template>

<script>
import './styles/global.css';
import HeaderGamesOn from './components/HeaderGamesOn.vue';
import HomeGameOn from './pages/HomeGameOn.vue';
import FooterGameOn from './components/FooterGameOn.vue';
export default {
  name: 'App',
  components: {
    HeaderGamesOn,
    HomeGameOn,
    FooterGameOn
}
}
</script>

<style lang="scss">

</style>
