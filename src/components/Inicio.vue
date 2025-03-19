<script setup>
import Menu from './Menu.vue';
import Restaurante from './Restaurante.vue';
</script>

<template>
  <div>
    <!-- Navbar -->
    <nav class="navbar navbar-expand-lg navbar-dark bg-primary">
      <div class="container">
        <a class="navbar-brand" href="#">WEBFOOD</a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav"
          aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
          <ul class="navbar-nav ms-auto">
            <li class="nav-item">
              <a class="nav-link" href="#" @click="mostrarSeccion('inicio')">Inicio</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#" @click="mostrarSeccion('restaurantes')">Restaurantes</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#" @click="mostrarSeccion('menu')">Menú</a>
            </li>
          </ul>
        </div>
      </div>
    </nav>

    <!-- Secciones -->
    <div class="container mt-5">
      
      <!-- Sección Inicio -->
      <div v-if="seccionActual === 'inicio'">
        <h1 class="text-center">BIENVENIDOS </h1><br>
        <p class="text-center">🍽️ "Descubre, saborea y disfruta: los mejores lugares para comer a tu alcance." 🌮🍕🥗</p>
        <div class="d-flex justify-content-center align-items-center" style="min-height: 0vh;">
          <img src="/logo.png" alt="Vue logo" class="img-fluid" style="max-width: 300px;">
        </div>
      </div>

      <!-- Sección Restaurantes -->
      <div v-if="seccionActual === 'restaurantes'">
        <Restaurante />
      </div>

      <!-- Sección Menú -->
      <div v-if="seccionActual === 'menu'">
        <Menu />
      </div>

    </div>

  </div>
</template>

<script>
export default {
  data() {
    return {
      seccionActual: 'inicio' // Sección inicial
    };
  },
  methods: {
    mostrarSeccion(seccion) {
      this.seccionActual = seccion;
    }
  }
};
</script>

<style>
.navbar {
  margin-bottom: 30px;
}
</style>
