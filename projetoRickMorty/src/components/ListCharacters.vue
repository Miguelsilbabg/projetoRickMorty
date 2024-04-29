<script setup>
const props = defineProps(["character"])
</script>

<template>
  <div class="col-md-4">
    <div class="card p-2 mb-3">
      <img :src="character.image" height="auto" alt="">
      <div class="card-body">
        <p class="text-center"><strong>Nome: {{ character.name }}</strong></p>
        <p>Status: {{ character.status }}</p>
        <p>Espécie: {{ character.species }}</p>
        <p>Genero: {{ character.gender }}</p>
        <p>Localização: {{ character.location.name }}</p>
      </div>
    </div>
  </div>
</template>

<style>

</style>