<template>
    <div class="hello">
      <h2>6. Dinamic Class</h2>
      <h4><i>:class=""</i></h4>
  
      <div>
        <h3 :class="[email.length < 5 ? 'red_signup' : 'green_signup']">Sign Up</h3>
        <input type="text" v-model="email" :class="{ red: email.length < 4 }" />
        <br />
        <button onclick="alert('signed up')" >
          Submit
        </button>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: "ClassDinamic",
    props: {
      msg: String,
    },
    data() {
      return {
        email: "",
      };
    },
  };
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped>
  .red {
    border: 2px solid red;
    outline: none;
  }
  
  .green {
    border: 2px solid green;
    outline: none;
  }

  .red_signup {
    color: red;
  }
  
  .green_signup {
    color: green;
  }
  </style>
  