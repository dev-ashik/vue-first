<template>
    <div class="hello">
      <h2>2. Read dinamic value</h2>
      <h2>{{ greeting }}</h2>

      <h4><i>v-model=""</i></h4>
      <input type="text" v-model="greeting">
    </div>
  </template>
  
  <script>
  export default {
    name: 'ReadData',
    props: {
      msg: String,
    },
    data() {
      return {
        greeting: "Hello Vue",
      }
    }
  }
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped>
  
  </style>
  