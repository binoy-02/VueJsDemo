<template>
    <h2 >DataBind</h2>
    <h2 v-bind:id="headingID">This is a example of Data Binding</h2>
    <button v-bind:=Disabled>Click Me</button>
  </template>
  
  <script>
  export default{
    name : "DataBinding",
    data(){return{
       headingID : 'heading',
       isDisabled : true,
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
  </style>
  
