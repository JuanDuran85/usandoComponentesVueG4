<template>
<main>
    <header class="text-white">
        <Lista :dataUser="personajes"/>
    </header>
  </main>
</template>

<script>
import Lista from './Lista.vue';

export default {
  name: 'Main',
  data() {
      return {
        personajes: [
            {nombre: "Rick Sanchez", src:"https://rickandmortyapi.com/api/character/avatar/1.jpeg"},
            {nombre: "Morty Smith", src:"https://rickandmortyapi.com/api/character/avatar/2.jpeg"},
            {nombre: "Summer Smith", src:"https://rickandmortyapi.com/api/character/avatar/3.jpeg"},
            {nombre: "Beth Smith", src:"https://rickandmortyapi.com/api/character/avatar/4.jpeg"},
            {nombre: 	"Alien Googah", src:"https://rickandmortyapi.com/api/character/avatar/13.jpeg"},
            {nombre: "Adjudicator Rick", src:"https://rickandmortyapi.com/api/character/avatar/8.jpeg"},
        ]
      }
  },
  components:{
      Lista
  }
}
</script>

<style scoped>
    header {
        margin: 0;
        padding: 0;
        background-image: url('https://rickandmortypod.com/wp-content/uploads/2018/11/cropped-RM_page-header_background1-3.png');
        background-repeat: no-repeat;
        background-size: cover;
        background-position: center top; 
    }
</style>
