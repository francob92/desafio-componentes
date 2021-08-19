<template>
  <div>
    <Personaje v-for="(personaje, index) in personajes" :key="index" :personaje="personaje" />
  </div>
</template>

<script>
import Personaje from './Personaje.vue';
export default {
  name: "App",
  components: { Personaje },
  data: () => ({
    personajes: [
      {
        nombre: "Rick Sanchez",
        src: "https://rickandmortyapi.com/api/character/avatar/1.jpeg",
      },
      {
        nombre: "Morty Smith",
        src: "https://rickandmortyapi.com/api/character/avatar/2.jpeg",
      },
    ],
  }),
};
</script>

<style>
body {
  background-image: url("../public/background.png");
}
</style>
