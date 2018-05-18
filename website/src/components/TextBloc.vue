<template lang="html">
     <div class="columns" id="text-bloc">
       <div class="column">
          <h1 class="title">{{title}}</h1>
          <p>{{content}}</p>
       </div>
     </div>
</template>

<script>
export default {
     name: 'TextBloc',
     props: ['title', 'content'],
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

     // MIXINS //
     // @mixin subtitle-text-style {
     //      letter-spacing: 2.5px!important;
     //      font-size: 14px!important;
     //      text-transform: uppercase!important;
     //      text-align: center;
     // }

     // STYLES //
     #text-bloc {
          padding: 75px 125px 75px 125px;
     }
     .title {
          font-family: $font-stack;
          color: $secondary-color;
          letter-spacing: 2px;
          text-align: center;
          // margin-top: 75px;
     }

     p {
          font-weight: bold!important;
          color: $primary-color;
          letter-spacing: 2.5px!important;
          font-size: 16px!important;
          text-align: center;
     }
</style>
