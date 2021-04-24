<template>
  <div>
    1. Local Variable Watcher
    <LocalVariableWatcher v-model="model1"></LocalVariableWatcher>
    {{ model1 }}
  </div>
</template>

<script>
import LocalVariableWatcher from "@/components/way1/LocalVariableWatcher";
export default {
  name: "App",
  components: {
    LocalVariableWatcher,
  },
  data() {
    return {
      model1: "",
    };
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  color: #2c3e50;
  margin-top: 60px;
}
</style>
