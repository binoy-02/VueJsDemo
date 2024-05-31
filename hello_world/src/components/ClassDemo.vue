<template>
    <h2>ClassBind</h2>
    <h2 class="Underline">Underlined Text</h2>  
    <h2 class="Underline" v-bind:class="status">Status</h2>
    <h2 v-bind:class="isPromoted && 'PromotedMovie'" >Promoted Movie</h2>
    <h2 v-bind:class="isNew && 'NewMovie'">New Movie</h2>
    <h2 v-bind:class="isSoldout ? 'SoldOut':'NewMovie'">SoldOut Movie</h2>
    <h2 v-bind:class="[isPromoted&&'NewMovie',isNew&&'PromotedMovie']">New Promoted Movie</h2>
    <h2 v-bind:class="[isPromoted && 'PromotedMovie',isSoldout?'SoldOut':'NewMovie']">Conditional Array Movie</h2>
    <h2 v-bind:class="{'NewMovie' : !SoldOut,
        'PromotedMovie' : isPromoted,
        'SoldOut' : SoldOut,}
        ">
      Object conditional movie
    </h2>
    
    
  </template>
  
  <script>
  export default{
    name : "classDemo",
    data(){return{
       headingID : 'heading',
       isDisabled : true,
       status: 'danger',
       isPromoted : false,
       isNew : true,
       isSoldout : false,
    }
    }

  }
  </script>
    
    
  <style>
  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }
  .Underline{
    text-decoration: underline;
    
  }

  .PromotedMovie{
   font-style :italic;
  }

  .NewMovie{
    color: green;
  }
  .SoldOut{
    color: red;
    position:bottom;
  }
  </style>
  
