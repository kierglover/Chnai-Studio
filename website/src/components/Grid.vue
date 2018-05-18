<template lang="html">
     <div class="tile is-ancestor">
               <div class="tile is-7">
                    <chnai-tile tileImage="https://images.unsplash.com/photo-1518553634183-40a6deeae021?ixlib=rb-0.3.5&ixid=eyJhcHBfaWQiOjEyMDd9&s=e16566688ea010dc0f73e4dac887ad10&auto=format&fit=crop&w=750&q=80" tileTitle="Testing prop" subtitle="Find out more" subtileLink="http://google.com">
                    </chnai-tile>
               </div>
               <div class="tile is-5 is-vertical">
                         <chnai-tile tileImage="https://images.unsplash.com/photo-1518553634183-40a6deeae021?ixlib=rb-0.3.5&ixid=eyJhcHBfaWQiOjEyMDd9&s=e16566688ea010dc0f73e4dac887ad10&auto=format&fit=crop&w=750&q=80" tileTitle="Testing prop" subtitle="Find out more" subtileLink="#">
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
          margin: 50px 100px 50px 100px!important;
     }
</style>
