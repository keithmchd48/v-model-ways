<template>
  <div>
    1. Local Variable Watcher
    <LocalVariableWatcher v-model="text1"></LocalVariableWatcher>
    {{ text1 }}
  </div>
  <div>
    2. Custom Method
    <CustomMethod v-model="text2"></CustomMethod>
    {{ text2 }}
  </div>
  <div>
    3. Powerful Computed property
    <PowerfulComputedProperty v-model="text3"></PowerfulComputedProperty>
    {{ text3 }}
  </div>
  <div>
    4. Named v-model
    <NamedVModel v-model:text="text5"></NamedVModel>
    {{ text5 }}
  </div>
</template>

<script>
import LocalVariableWatcher from "@/components/way1/LocalVariableWatcher";
import CustomMethod from "@/components/way2/CustomMethod";
import PowerfulComputedProperty from "@/components/way3/PowerfulComputedProperty";
import NamedVModel from "@/components/way4/NamedVModel";

export default {
  name: "App",
  components: {
    LocalVariableWatcher,
    CustomMethod,
    PowerfulComputedProperty,
    NamedVModel,
  },
  data() {
    return {
      text1: "",
      text2: "",
      text3: "",
      text4: "",
      text5: "",
      text6: "",
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
