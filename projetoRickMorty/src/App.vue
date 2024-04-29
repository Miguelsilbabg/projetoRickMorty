<script setup>
import {ref} from 'vue'

let num = ref(0)

</script>

<template>
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark border-bottom border-body">
    <div class="container-fluid">
      <RouterLink class="navbar-brand" to ="/">Rick Morty</RouterLink>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="nav-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item">
            <RouterLink class="nav-link" aria-current="page" to="/">Inicio</RouterLink>
          </li>
          <li class="nav-item">
            <RouterLink class="nav-link" aria-current="page" to="/about">Sobre</RouterLink>
          </li>
        </ul>
      </div>
    </div>
  </nav>
  
    <div class="main">
      <RouterView></RouterView>
    </div>

    <footer class="bg-dark text-light">
      <div>Unimar | ADS 2024| {{ new Date().getFullYear() }}</div>
    </footer>
</template>

<style>
footer{
  position: fixed;
  bottom: 0;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  height: 50px;
}
</style>
