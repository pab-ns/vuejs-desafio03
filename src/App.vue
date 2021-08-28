<template>
  <div>
    <!-- <h1>PERSONAJES</h1> -->
    <Personajes />
  </div>
</template>

<script>
/* 1. Importar componente (tal cual como fue exportado) */
import Personajes from "./components/Personajes.vue";

export default {
  name: "App",
  components: { Personajes },
  data: () => ({}),
};
</script>

<style>
body {
  background-image: url(./assets/cropped-RM_page-header_background1-3.png);
  background-size: cover;

  color: green;
  font-size: 1.5rem;
  font-weight: bold;
  font-family: sans-serif;
}
</style>
