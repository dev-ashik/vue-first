<template>
  <HelloWorld/>
  <hr>
  <ReadData/>
  <hr>
  <VCondition/>
  <hr>
  <VShow/>
  <hr>
  <VBind/>
  <hr>
  <ClassDinamic/>
  <hr>
  <VText/>
  <hr>
  <LoopVue/>
</template>

<script>
import ClassDinamic from './components/ClassDinamic.vue';
import HelloWorld from './components/HelloWorld.vue'
import LoopVue from './components/LoopVue.vue';
import ReadData from './components/ReadData.vue';
import VBind from './components/VBind.vue';
import VCondition from './components/VCondition.vue';
import VShow from './components/VShow.vue';
import VText from './components/VText.vue';

export default {
  name: 'App',
  components: {
    HelloWorld,
    ReadData,
    VCondition,
    VShow,
    VBind,
    ClassDinamic,
    VText,
    LoopVue
}
}
</script>


<!-- Time: 34:02 -->
<style>
#app {
  /* font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px; */
}
</style>
