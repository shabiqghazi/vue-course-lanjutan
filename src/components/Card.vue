<template>
  <div class="card shadow mb-3" style="max-width: 18rem">
    <div class="card-header">
      <slot name="card-header"></slot>
    </div>
    <div class="card-body">
      <slot></slot>
    </div>
    <div class="card-footer">
      <slot name="card-footer"></slot>
    </div>
  </div>
</template>

<script>
export default {
  name: "CardComponent",
};
</script>

<style scoped>
</style>