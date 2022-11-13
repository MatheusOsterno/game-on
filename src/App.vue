<template>
  <div id="app">
    <HeaderGamesOn />
    <HomeGameOn />
    <h1>Lançamentos</h1>
    <CardGamesOn />
    <h1>Promoções</h1>
    <CardGamesOn />
    <h1>Multiplayer</h1>
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


h1 {
  margin-top: 20px;
  
  background: linear-gradient(45deg, #058905, rgb(12, 222, 82));
  border: solid black;
  padding: 20px;
  font-family: 'Courier New', Courier, monospace;
  display: flex;
  align-items: center;
  justify-content: center;
}

</style>
