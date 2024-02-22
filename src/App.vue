<script setup>
import CabecalhoPokedex from './components/Cabecalho.vue'
import BodyPokedex from './components/Body.vue'
</script>

<template>
  <body>
    <header>
      <div class="podexex_cabecalho">
        <cabecalho-pokedex />
      </div>
    </header>

    <div id="body_pokedex">
      <body-pokedex />
    </div>

  </body>
</template>

<style scoped>
.podexex_cabecalho {
  /* display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 20vh; */
  position: fixed;
}
</style>
