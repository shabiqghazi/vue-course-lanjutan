<template>
  <h4>Component E</h4>
  <p>user: {{ username }}</p>
</template>

<script>
  export default {
    name: 'ComponentE',
    inject: ['username']
  }
</script>

<style scoped>

</style>