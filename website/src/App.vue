<template>
  <div id="app">
       <chnai-navbar></chnai-navbar>
       <chnai-hero title="Mothers Day Collection" subtitle="View More"></chnai-hero>
       <text-bloc title="Hand Crafted Stationery" content="We are a creative couple with a passion for bringing Cambodia modern stationery, wedding invitations and greeting cards. All our collections are designed in our small studio in Phnom Penh."></text-bloc>
       <chnai-grid></chnai-grid>
       <reverse-grid></reverse-grid>
  </div>
</template>

<script>
import Nav from './components/Nav.vue'
import Hero from './components/Hero.vue'
import Grid from './components/Grid.vue'
import ReverseGrid from './components/Reverse-Grid.vue'
import TextBloc from './components/TextBloc.vue'
export default {
name: 'app',
components: {
     'chnai-navbar': Nav,
     'chnai-hero': Hero,
     'chnai-grid': Grid,
     'reverse-grid': ReverseGrid,
     'text-bloc': TextBloc,
     },
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<style lang="sass">
@import url('https://fonts.googleapis.com/css?family=Old+Standard+TT');

// VARIABLES //
$body-color: #FDFDFD;

// MIXINS //

// STYLES //

#app {
     background-color: $body-color;
}

</style>
