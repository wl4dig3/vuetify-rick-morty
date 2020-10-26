<template>
  <div>
    <h1>{{titlee}}</h1>
    <v-container>
      <v-row>
        <v-col v-for="(personaje, i) in personajes"
            :key="i">
          <v-card
            class="mx-auto"
            max-width="344"
            
          >
            <v-img :src="personaje.imagen" height="200px"></v-img>

            <v-card-title> {{ personaje.nombre }}</v-card-title>

            <!-- <v-card-subtitle> 1,000 miles of wonder </v-card-subtitle> -->
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  data: () => ({
    titlee:'Lady and gentleman, we introduce to Rick and Morty',
    personajes: [
      {
        id: 1,
        nombre: "Morty",
        imagen: "https://rickandmortyapi.com/api/character/avatar/2.jpeg",
      },
      {
        id: 2,
        nombre: "Rick",
        imagen: "https://rickandmortyapi.com/api/character/avatar/1.jpeg",
      },
      {
        id: 3,
        nombre: "Summer",
        imagen: "https://rickandmortyapi.com/api/character/avatar/3.jpeg",
      },
      {
        id: 4,
        nombre: "Beth",
        imagen: "https://rickandmortyapi.com/api/character/avatar/4.jpeg",
      },
      {
        id: 5,
        nombre: "Jerry",
        imagen: "https://rickandmortyapi.com/api/character/avatar/5.jpeg",
      },
      {
        id: 6,
        nombre: "Alien Spa",
        imagen: "https://rickandmortyapi.com/api/character/avatar/361.jpeg",
      },
    ],
  }),
};
</script>