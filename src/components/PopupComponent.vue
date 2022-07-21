<template>
  <div class="border rounded border-dark p-3 col-4">
    <h3>Popup</h3>
    <input class="form-control mb-2" type="text" v-model="name">
    <button class="btn btn-danger" @click="$emit('close', name)">close</button>
  </div>
</template>

<script>
  export default {
    name: 'PopupComponent',
    data(){
      return {
        name : 'Shabiq',
      }
    },
    emits: {
      close: (name) => {
        if(!name){
          return false
        } else {
          return true
        }
      }
    }
  }
</script>

<style scoped>

</style>