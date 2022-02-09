<template>
  <div id="app">
    <header-container/>
    <main-container/>
    <footer-box/>
  </div>
</template>

<script>
import HeaderContainer from './components/HeaderContainer.vue'
import MainContainer from './components/MainContainer.vue'
import FooterBox from './components/FooterBox.vue'


export default {
  name: 'App',
  components: {
    HeaderContainer,
    MainContainer,
    FooterBox
  }
}
</script>

<style lang="scss">
@import './style/body.scss';
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@400;500&display=swap');
</style>