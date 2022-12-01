<template>
    <div class="hello">
      <h2>7. vue text</h2>
      <h4><i>v-text="email", v-once</i></h4>
  
      <div>
        <p>{{ email }}</p>
        <p v-text="email"></p>
        <p v-once>{{ email }}</p>
        <input type="text" v-model="email"/>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: "VText",
    props: {
      msg: String,
    },
    data() {
      return {
        email: "something@test.com",
      };
    },
  };
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped>
  
  </style>
  