<script setup>
import HelloWorld from "./components/HelloWorld.vue";
import TheHeader from "./components/TheHeader.vue";
import TheFooter from "./components/TheFooter.vue";
import { ref } from "vue";



const datos = ref ({
    nombre: "Pepe",
    edad: 30,
  },
    {
      nombre: "Laura",
      edad: 45,
    },
    { nombre: "Juanca", edad: 3 });
</script>

<template>
  <div>
    <TheHeader />
    <a href="https://vitejs.dev" target="_blank">
      <img src="./assets/Screenshot-gafas.png" class="logo" alt="imagen random" />
    </a>
  </div>
  <HelloWorld :datos="datos" />
  <TheFooter />
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
}

.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}

.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
