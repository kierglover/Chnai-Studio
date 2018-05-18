<template lang="html">

     <section class="hero-cta">
          <nav class="level">
               <div class="level-item">
                    <div>
                         <h2>Chnai Studio</h2>
                    </div>
               </div>
              <div class="level-item has-text-centered">
                   <div>
                       <a class="button is-medium">Stationery</a>
                   </div>
              </div>
              <div class="level-item has-text-centered">
                   <div>
                       <a class="button is-medium">Wedding Suites</a>
                   </div>
              </div>
              <div class="level-item has-text-centered">
                   <div>
                        <a class="button is-medium">Greetings Cards</a>
                   </div>
              </div>
         </nav>
    </section>

</template>

<script>
export default {
     name: 'HeroCta'
}
</script>

<style lang="sass" scoped>
// VARIABLES //
$font-stack: 'Old Standard TT', serif;
$secondary-font: 'Lato', sans-serif;
$primary-color: rgba(211, 195, 192, 100);
$secondary-color: rgba(125, 112, 109, 100);
$tertiary-color: rgba(228, 219, 191, 100);

// MIXINS //
@mixin custom-btn {
     border: 2px solid!important;
     color: $primary-color!important;
     border-radius: 0px!important;
     width: 30vh!important;
     height: 8vh!important;
     font-family: $secondary-color!important;
     text-transform: uppercase;
     }
          // STYLES //
          .hero-cta {
               padding: 50px 125px 50px 125px;
          }

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
</style>
