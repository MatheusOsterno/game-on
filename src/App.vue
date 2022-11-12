<template>
  <div id="app">
    <HeaderGamesOn />
    <HomeGameOn />
  </div>
</template>

<script>
import './styles/global.css';
import HeaderGamesOn from './components/HeaderGamesOn.vue';
import HomeGameOn from './pages/HomeGameOn.vue';

export default {
  name: 'App',
  components: {
    HeaderGamesOn,
    HomeGameOn
}
}
</script>

<style lang="scss">

</style>
