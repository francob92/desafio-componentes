<template>
  <div>
    <img :src="personaje.src" alt="personaje">
    <p>{{personaje.nombre}}</p>
  </div>
</template>

<script>
export default {
  name: "Personaje",
  
  props: { personaje: { type: Object } },
};
</script>

<style>
div {
  color: green;
}
p {
  display: inline-block;
}
img {
  border-radius: 50%;
}
</style>
