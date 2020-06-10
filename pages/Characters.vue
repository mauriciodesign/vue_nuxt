<template>
  <v-app>
    <v-container>
      <v-row>
        <v-col
          v-for="(character, index) in characters"
          :key="index"
          cols="12"
          lg="4"
          md="4"
          sm="4"
        >
          <v-card>
            <v-img
              :src="character.imagen"
            />
            <v-card-title>{{ character.nombre }}</v-card-title>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </v-app>
</template>

<script>
export default {
  name: 'App',
  data: () => ({
    drawer: false,
    characters: [
      {
        id: 1,
        nombre: 'Morty',
        imagen: 'https://rickandmortyapi.com/api/character/avatar/2.jpeg'
      },
      {
        id: 2,
        nombre: 'Rick',
        imagen: 'https://rickandmortyapi.com/api/character/avatar/1.jpeg'
      },
      {
        id: 3,
        nombre: 'Summer',
        imagen: 'https://rickandmortyapi.com/api/character/avatar/3.jpeg'
      },
      {
        id: 4,
        nombre: 'Beth',
        imagen: 'https://rickandmortyapi.com/api/character/avatar/4.jpeg'
      },
      {
        id: 5,
        nombre: 'Jerry',
        imagen: 'https://rickandmortyapi.com/api/character/avatar/5.jpeg'
      }
    ]
  })
}
</script>
