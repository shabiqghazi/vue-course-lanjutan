<template>
  <div>
    <div class="card col-6">
      <div class="card-body">
        <p>Tab C</p>
        <input
          class="form-control"
          type="text"
          placeholder="Nama"
          aria-label="default input example"
          v-model="name"
        />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "TabC",
  data() {
    return {
      name: "",
    };
  },
};
</script>

<style scoped>
</style>