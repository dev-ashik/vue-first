<template>
    <div class="hello">
      <h2>4. Vue Show</h2>
      <h4><i>v-show=""</i></h4>

      <div v-show="(count === 1)">
        <h3>I am here.</h3>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'VShow',
    props: {
      msg: String,
    },
    data() {
      return {
        count: 1
      }
    }
  }
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped>
  
  </style>
  