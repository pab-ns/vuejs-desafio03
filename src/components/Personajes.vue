<template>
  <div>
    <ul>
      <li v-for="(personaje, $index) in personajes" :key="$index">
        <img :src="personaje.src" class="default" width="100" />
        {{ personaje.nombre }}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "Personajes",
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
      {
        nombre: "Summer Smith",
        src: "https://rickandmortyapi.com/api/character/avatar/3.jpeg",
      },
      {
        nombre: "Beth Smith",
        src: "https://rickandmortyapi.com/api/character/avatar/4.jpeg",
      },
      {
        nombre: "Jerry Smith",
        src: "https://rickandmortyapi.com/api/character/avatar/5.jpeg",
      },
    ],
  }),
};
</script>

<style>
ul {
  list-style: none;
}

ul li {
  padding: 0.7rem 0;
}

ul li img {
  vertical-align: middle;
}

.default {
  border-radius: 50%;
}
</style>
