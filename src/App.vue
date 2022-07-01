<template>
  <div id="app">

    <TheHeader></TheHeader>
    <TheJumbotron></TheJumbotron>
    <TheMain></TheMain>
    <TheFooter></TheFooter>
    
  </div>
</template>

<script>
import TheHeader from './components/TheHeader.vue';
import TheJumbotron from './components/TheJumbotron.vue'
import TheMain from './components/TheMain.vue';
import TheFooter from './components/TheFooter.vue';

export default {
  name: 'App',
  components: {
    TheHeader,
    TheJumbotron,
    TheMain,
    TheFooter
}
}
</script>

<style lang="scss">
@import "assets/scss/main.scss";
#app {
  @import url('https://fonts.googleapis.com/css2?family=Fredoka:wght@400;700&family=Poppins&display=swap');
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
</style>
