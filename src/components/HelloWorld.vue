<script setup>
import { ref } from 'vue'
const name=ref("")

defineProps({
  msg: String,
})

const age = ref(0)

</script>

<template>
  <label> Insert name: 
  <input type="text" v-model="name"></label>
  <h1>{{ name }} has {{ age }} years old</h1>

  <div class="card">
    <button type="button" @click="age++">add years to {{ name }}</button>
   
  </div>

  
</template>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>
