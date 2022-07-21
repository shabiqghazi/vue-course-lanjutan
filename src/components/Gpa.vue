<template>
  <h3 v-for="student in students" :key="student.fullName">
    <slot :fullName="student.fullName" :gpa="student.gpa"></slot>
  </h3>
  <!-- <slot></slot> -->
</template>

<script>
export default {
  name: "GpaComponent",
  data() {
    return {
      students: [
        {
          fullName: "Shabiq Ghazi Arkaan",
          gpa: 3.97,
        },
        {
          fullName: "Hendra Setiawan",
          gpa: 3.9,
        },
        {
          fullName: "Mohammad Ahsan",
          gpa: 3.88,
        },
      ],
    };
  },
};
</script>

<style scoped>
</style>