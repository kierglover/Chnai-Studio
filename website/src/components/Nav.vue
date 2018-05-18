<template lang="html">

     <nav class="navbar" role="navigation" aria-label="main navigation">
       <div class="navbar-brand">
         <a class="navbar-item" href="https://bulma.io">Chnai Studio</a>
       </div>
     </nav>

</template>

<script>
export default {
}
</script>

<style lang="sass" scoped>

$font-stack: 'Old Standard TT', serif;
$primary-color: #D3C3C0;
$secondary-color: white;

@mixin body-margin {
     margin-left: 89px;
     margin-right: 89px;
     }

     .navbar {
          background-color: $primary-color;
          height: 15vh;
          padding-top: 35px;
          padding-bottom: 35px;
     }

     .navbar-item {
          color: $secondary-color;
          font-family: $font-stack;
          @include body-margin;
          font-size: 27px;
          letter-spacing: 2px;
     }
</style>
