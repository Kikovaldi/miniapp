

<template>
  <form>
    <input type="number" v-model="amount"/>
    <button @click.prevent="addMoney">Submit</button>
  </form>

 <Box :listaAmounts="total" />
</template>

<script>
import Box from "./components/box.vue";
import Button from "./components/Button.vue"
export default {
name: "App",
  components: { Button, Box }, 
  data() { 
    return {
        amount: "",
      total: [],
      totalSuma:"",
    
    }},

    methods: {
      addMoney(){
        this.total.push(this.amount)
        console.log(this.total)
        return this.total

    },
    addTotal(){

    }
  }}
 
</script>


<style>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
