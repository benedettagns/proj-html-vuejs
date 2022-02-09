<template>
  <div id="app">
    <header-container/>
    <main-container/>
    <results-container/>
    <performance-box/>
    <footer-box/>
  </div>
</template>

<script>
import HeaderContainer from './components/HeaderContainer.vue'
import MainContainer from './components/MainContainer.vue'
import FooterBox from './components/FooterBox.vue'
import ResultsContainer from './components/ResultsContainer.vue'
import PerformanceBox from './components/PerformanceBox.vue'


export default {
  name: 'App',
  components: {
    HeaderContainer,
    MainContainer,
    FooterBox,
    ResultsContainer,
    PerformanceBox
  }
}
</script>

<style lang="scss">
@import './style/body.scss';
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@400;500&display=swap');
</style>