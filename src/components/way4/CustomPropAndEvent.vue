<template>
  <input type="text" :value="text" @input="onInput" />
</template>

<script>
export default {
  model: {
    prop: "text",
    event: "update",
  },
  props: {
    text: {
      type: String,
      default: "",
    },
  },
  methods: {
    onInput(value) {
      this.$emit("update", value);
    },
  },
};
</script>
