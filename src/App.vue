<template>
  <div id="app">
    <div><input v-model="base" /> Число</div>
    <div><input v-model="howMany" /> Степень</div>
    <template v-for="i in +howMany">
      <Deg :base="+base" :exp="9+i" :key="i" />
    </template>
  </div>
</template>

<script>
import Deg from "./Deg";
export default {
  name: "App",
  components: {
    Deg,
  },
  data() {
    return {
      base: 2,
      howMany: 2,
    };
  },
  methods: {},
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.flex {
  display: flex;
}
</style>
