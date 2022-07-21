<template>
  <h3>Component D</h3>
  <component-e />
</template>

<script>
  import ComponentE from "./ComponentE.vue";
  export default {
    name: 'ComponentD',
    components: {
      ComponentE
    }
  }
</script>

<style scoped>

</style>