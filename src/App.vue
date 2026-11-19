<script setup>
import HelloWorld from './components/HelloWorld.vue'
import {getPokemon} from './api/pokeapi.js'

</script>

<template>
  <div v-if="pokemon">
    <h1>{{ pokemon.name }}</h1>
    <p># {{ pokemon.id }}</p>
    <img :src="pokemon.sprites.front_default" :alt="pokemon.name" />
  </div>
  <button @click="cambiarPokemon">Otro Pokémon</button>
</template>



