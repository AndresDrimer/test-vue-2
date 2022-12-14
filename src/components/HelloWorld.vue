<script setup>
import { ref } from 'vue'
const name = ref("")
const age = ref(0)
const props = defineProps ({ datos: String })
</script>

<template>
  <label> Insert name:
    <input type="text" v-model="name"></label>
  <h1>{{ name }} has {{ age }} years old</h1>

  <div class="card">
    <button type="button" @click="age++">add years to {{ name }}</button>

  </div>
  <div v-for="dato in datos" :key="dato.nombre"> {{datos}}</div>


</template>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>
