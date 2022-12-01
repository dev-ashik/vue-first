<template>
  <div class="hello">
    <h2>5. Vue Bind</h2>
    <h4><i>v-bind:dispaly="email.length &gt; 2"</i></h4>

    <div>
      <h3>Sign Up</h3>

      <input type="text" v-model="email" />
      <br />
      <button onclick="alert('signed up')" v-bind:disabled="email.length < 2">
        Submit
      </button>
      <!-- same -->
      <button onclick="alert('signed up')" :disabled="email.length < 2">
        Submit
      </button>
    </div>
  </div>
</template>

<script>
export default {
  name: "VBind",
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
</style>
