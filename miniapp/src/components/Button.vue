<template>
    <button>{{ text }}</button>
  </template>
  
  <script>
  export default {
    name: "Button",
    data() {
      return {
        text: "Enviar",
      };
    },
  };
  </script>
  
  <style>
  button {
    background-color: rgb(6, 125, 86);
    border-radius: 0.2rem;
    border: 0;
    padding: 0.2rem 1rem 0.2rem 1rem;
    color: rgb(255, 255, 255);
    height: 50px;
    width: 100px;
  }
  button:hover  {
    background-color: rgb(104, 196, 224);
  }
  </style>
  