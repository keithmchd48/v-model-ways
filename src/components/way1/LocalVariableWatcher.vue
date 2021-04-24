<template>
  <input type="text" v-model="model" />
</template>

<script>
export default {
  name: "LocalVariableWatcher",
  props: {
    value: {
      type: String,
      default: "",
    },
  },
  data() {
    return {
      model: this.value,
    };
  },
  watch: {
    model(currentValue) {
      this.$emit("input", currentValue);
    },
  },
};
</script>
