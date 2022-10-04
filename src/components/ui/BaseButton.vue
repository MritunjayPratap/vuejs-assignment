<template>
  <button>
    <slot></slot>
  </button>
</template>

<script>
export default {
  props: {
    backgroundColor: {
      type: String,
      required: false,
      default: "#f4f6f8",
    },
  },
};
</script>

<style scoped>
button {
  background-color: v-bind(backgroundColor);
  display: inline-flex;
  border: none;
  border-radius: 0.5rem;
  cursor: pointer;
}
</style>
