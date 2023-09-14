<template>

  <div>
    <p v-for="item in listaAmounts"> {{ item }}</p>
  </div>
  </template>
  
  <script>
  export default {
    name: "Box",
    props: ["listaAmounts"]
  };
  </script>
  
  <style></style>
  