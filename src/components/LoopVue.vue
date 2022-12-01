<template>
  <div class="hello">
    <h2>8. Loop</h2>
    <h4><i></i></h4>

    <ul>
      <li v-for="cat in cats" v-bind:key="cat">{{ cat.name }}</li>
    </ul>

    <div>
      <h3>Add new Kitty</h3>
      <input type="text" v-model="newCat" v-on:keyup.enter="addKitty" />
      <button v-on:click="addKitty">
        + add
      </button>
    </div>
  </div>
</template>

<script>
export default {
  name: "LoopVue",
  props: {
    msg: String,
  },
  data() {
    return {
      cats: [
        {name: "Kitkat"}, 
        {name: "Fish"}, 
        {name: "Henry"}, 
        {name: "Bosco"},
    ],
      newCat: "",
    };
  },
  methods: {
    addKitty() {
        return this.cats.push({name: this.newCat});
    }
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped></style>
