<template lang="html">
          <div class="tile is-parent">
               <div class="tile is-child box">
                    <img v-bind:src="tileImage" alt="tileImage" class="image">
                    <div class="overlay">
                         <h2>{{tileTitle}}</h2>
                         <hr>
                         <a class="tileSubtitle" v-bind:href="subtileLink" target="_blank">{{subtitle}}</a>
                    </div>
               </div>
          </div>
</template>

<script>
export default {
     props: ['tileImage', 'tileTitle', 'subtitle', 'subtileLink'],
data() {
     return {
          // subtitle: 'Mothers Day Collection'
          }
     }
}
</script>

<style lang="sass" scoped>
// VARIABLES
$font-stack: 'Old Standard TT', serif;
$secondary-font: 'Lato', sans-serif;
$tertiary-color: rgba(228, 219, 191, 100);
$secondary-color: rgba(125, 112, 109, 100);

// MIXINS
@mixin subtitle-text-style {
     font-weight: bold!important;
     color: $tertiary-color!important;
     letter-spacing: 2.5px!important;
     font-size: 16px!important;
     text-transform: uppercase!important;
}
     //STYLES
     h2 {
          font-family: $font-stack;
          color: $secondary-color;
          font-size: 27px!important;
     }

     .image {
          width: 100%;
          opacity: 1;
          display: block;
          height: 75vh;
          transition: .5s ease;
          backface-visibility: hidden;
     }

     .tile.is-child {
          padding: 0px 0px 0px 0px;
          position: relative;
     }

     .overlay {
       transition: .5s ease;
       opacity: 0;
       position: absolute;
       top: 50%;
       left: 50%;
       transform: translate(-50%, -50%);
       -ms-transform: translate(-50%, -50%);
       text-align: center;
     }

     .box {
          box-shadow: none!important;
          height: 50vh;
     }

     .box:hover .image {
     opacity: 0.2;
     }

     .box:hover .overlay {
     opacity: 1;
     }

     .tileSubtitle {
     font-family: $secondary-font;
     margin-top: 35px!important;
     @include subtitle-text-style;
     }
</style>
