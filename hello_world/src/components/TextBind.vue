<template>
    <div>{{ greet }} </div>
    <div v-text= "salu"> </div>
    <div>{{ name }}</div>
  </template>
  
  <script>
  export default {
    name: 'TextBinding',
    data(){return{
      name : "Binoy",
      greet : "Hello",
      salu : "Mr"  };
  },
  };
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
  