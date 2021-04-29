<template>
  <input type="text" :value="text" @input="onInput" />
</template>

<script>
export default {
  props: {
    text: {
      type: String,
      value: "",
    },
  },
  methods: {
    onInput(event) {
      this.$emit("update:text", event.target.value);
    },
  },
};
</script>
