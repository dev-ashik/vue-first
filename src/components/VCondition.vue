<template>
    <div class="hello">
      <h2>3. Vue Condition</h2>
      <h4><i>v-if=""</i></h4>

      <div v-if="(count === 1)">
        <h3>One</h3>
      </div>
      <div v-else-if="(count === 2)">
        <h3>Two</h3>
      </div>
      <div v-else>
        <h3>{{ count }}</h3>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'VCondition',
    props: {
      msg: String,
    },
    data() {
      return {
        count: 0
      }
    }
  }
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped>
  
  </style>
  