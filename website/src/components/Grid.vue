<template lang="html">
     <div class="tile is-ancestor">
               <div class="tile is-7">
                    <chnai-tile tileImage="./src/static/wedding-invitations-with-chnai-phnom-penh.jpg" tileTitle="Wedding Suites" subtitle="Find out more" subtileLink="http://google.com">
                    </chnai-tile>
               </div>
               <div class="tile is-5 is-vertical">
                         <chnai-tile tileImage="./src/static/custom-wedding-invitations-phnom-penh.jpg" tileTitle="Stationery" subtitle="Find out more" subtileLink="#">
                         </chnai-tile>
               </div>
     </div>
</template>

<script>
import Tiles from './Tiles.vue'
export default {
     components: {
          'chnai-tile': Tiles,
     },
}
</script>

<style lang="sass" scoped>
     .tile.is-ancestor {
          margin: 0px 100px 50px 100px!important;
     }
</style>
