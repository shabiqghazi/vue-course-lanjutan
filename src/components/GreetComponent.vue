<template>
  <h2>Hello, I'm {{ name }} </h2>
  <p>I'm student at {{ collegeName }} </p>
  <hr>
</template>

<script>

export default {
  name : "GreetComponent",
  props : ['name', 'collegeName']
}
</script>

<style>

</style>