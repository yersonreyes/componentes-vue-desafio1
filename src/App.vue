<template>
  <div id="app">
       <Avatar
      v-for="({nombre, src}, $index) of personajes"
      :key="$index"
      :nombre="nombre"
      :imagen="src"
    />
  </div>
</template>

<script>
import Avatar from './components/Avatar'

export default {
  name: 'App',
  components: {Avatar},
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

}
</script>

<style>
  body{
    background: url('https://rickandmortypod.com/wp-content/uploads/2018/11/cropped-RM_page-header_background1-3.png');
    margin: 0;
    padding: 0;
  }
</style>
