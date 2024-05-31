<template>
    <h2>ClassBind</h2>
    <h2 class="Underline">Underlined Text</h2>  
    <h2 v-bind:class="status">Status</h2>
  </template>
  
  <script>
  export default{
    name : "classDemo",
    data(){return{
       headingID : 'heading',
       isDisabled : true,
       status: 'danger',
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
  </style>
  
