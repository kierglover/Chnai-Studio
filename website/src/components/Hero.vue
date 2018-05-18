<template lang="html">
     <section class="hero is-medium is-bold">
       <div class="hero-body">
               <div class="container animated fadeIn" id="image-overlay">
                    <h2 class="subtitle">Introducing Our</h2>
                    <h1 class="title">{{title}}</h1>
                    <a class="button is-medium">{{subtitle}}</a>
               </div>
       </div>
       <hr class="full-width-rule">
       <hero-cta></hero-cta>
      <hr class="full-width-rule">
     </section>
</template>

<script>
import HeroCta from './HeroCta.vue'
export default {
     name: 'hero',
     components: {
          'hero-cta': HeroCta,
     },
     props: ['title', 'subtitle'],
     data() {
          return {
               // message: 'Mothers Day Collection'
          }
     }
}

</script>

<style lang="sass" scoped>
// VARIABLES //
$font-stack: 'Old Standard TT', serif;
$secondary-font: 'Lato', sans-serif;
$primary-color: rgba(211, 195, 192, 100);
$secondary-color: rgba(125, 112, 109, 100);
$tertiary-color: rgba(228, 219, 191, 100);

//MIXINS //
@mixin border-radius($radius) {
  -webkit-border-radius: $radius;
     -moz-border-radius: $radius;
      -ms-border-radius: $radius;
          border-radius: $radius;
}

@mixin subtitle-text-style {
     font-weight: bold!important;
     color: white!important;
     letter-spacing: 2.5px!important;
     font-size: 14px!important;
     text-transform: uppercase!important;
     text-align: center;
}

@mixin hr-style1 {
     border-top: 1px solid rgba($primary-color, .5);
     margin: 0px 100px 0px 100px;
}

@mixin custom-btn {
     border: 2px solid!important;
     color: $primary-color!important;
     border-radius: 0px!important;
     width: 30vh!important;
     height: 8vh!important;
     font-family: $secondary-color!important;
     text-transform: uppercase;
          }

     //STYLES//
     h2 {
          font-family: $font-stack;
          color: $secondary-color;
          font-size: 27px!important;
     }

          .button.is-medium {
               @include custom-btn;
               font-size: 16px!important;
               letter-spacing: 2px!important;
               -webkit-transition: background-color 0.4s; /* Safari */
               transition: background-color 0.4s;
          }

          .button.is-medium:hover {
               background-color: $tertiary-color;
               border: none!important;
               color: white!important;
     }

     .hero-body {
          margin: 50px 100px 50px 100px;
          background-image: url("https://images.unsplash.com/photo-1522827489705-0616731a52a8?ixlib=rb-0.3.5&ixid=eyJhcHBfaWQiOjEyMDd9&s=bc3136a9d7f722e99966b0559414aee7&auto=format&fit=crop&w=1354&q=80");
          // ./src/static/custom-stationary-phnom-penh.jpg //
          background-repeat: no-repeat center center fixed;
          background-size: cover;
     }

     #image-overlay {
          padding: 25px 50px 25px 50px;
          text-align: center;
          width: 45%;
          height: 35vh;
          background-color: rgba($primary-color, .95);
          @include border-radius(10px);
     }

     .title {
          font-family: $font-stack;
          color: white!important;
          letter-spacing: 2px;
     }

     .subtitle {
          font-family: $secondary-font;
          margin-top: 25px!important;
          margin-bottom: 50px!important;
          @include subtitle-text-style;
     }

     .full-width-rule {
          @include hr-style1;
     }

</style>
