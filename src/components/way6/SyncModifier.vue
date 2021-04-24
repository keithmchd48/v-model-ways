<template>
  <input type="text" :value="text" @input="onInput" />
</template>

<script>
export default {
  props: {
    text: {
      type: String,
      default: "",
    },
  },
  methods: {
    onInput(value) {
      this.$emit("update:text", value.target.value);
    },
  },
};
</script>
