<template>
  <input type="text" :value="modelValue" @input="onInput" />
</template>

<script>
export default {
  name: "CustomMethod",
  props: {
    modelValue: {
      type: String,
      default: "",
    },
  },
  methods: {
    onInput(event) {
      // const val = event.target.value;
      this.$emit("update:modelValue", event.target.value);
    },
  },
};
</script>
