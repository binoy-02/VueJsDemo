<template>
    <div>{{ greet }} </div>
    <div v-html= "salu"> </div>
    <div>{{ name }}</div>
    <div v-html="hack"></div>
  </template>
  
  <script>
  export default {
    name: 'HtmlBinding',
    data(){return{
      name : "BINOY",
      greet : "HI",
      salu : '<b>MR</b>',
      hack : <a href="#" onclick ='alert("You have been hacked")'>Click Here</a>
      
    };
      
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
  