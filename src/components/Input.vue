<template>
  <div>
    <input
      class="form-control"
      type="text"
      placeholder="Default input"
      aria-label="default input example"
      :value="modelValue"
      @input="$emit('update:modelValue', $event.target.value)"
    />
  </div>
</template>

<script>
export default {
  name: "InputComponent",
  props: {
    modelValue: String,
  },
};
</script>

<style scoped>
</style>