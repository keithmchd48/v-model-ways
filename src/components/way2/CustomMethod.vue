<template>
  <input type="text" :value="value" @input="onInput" />
</template>

<script>
export default {
  name: "CustomMethod",
  props: {
    value: {
      type: String,
      default: "",
    },
  },
  methods: {
    onInput(event) {
      // const val = event.target.value;
      this.$emit("input", event);
    },
  },
};
</script>
