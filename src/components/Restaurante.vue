<template>
  <div >
    <!-- Encabezado -->
    <div class="d-flex justify-content-between align-items-center">
      <img src="/logo.png" alt="Logo WebFood" class="logo img-fluid" style="max-height: 90px;">
      <div class="input-group w-50">
        <input type="text" class="form-control" placeholder="Buscar restaurantes" />
        <button class="btn btn-outline-secondary" type="button">
          🔍
        </button>
      </div>
    </div>

    <!-- Título -->
    <h1 class="text-center mt-4">CAFÉ COLÓN</h1>
    <div class="text-center">
      <span class="badge bg-warning text-dark">✨</span>
      <span class="badge bg-warning text-dark">✨</span>
    </div>

    <!-- Imagen con descripción -->
    <div class="card mt-4">
      <img src="/colon.png" class="img-fluid" alt="Café Colón" />
      <div class="card-body text-center">
        <h2 class="card-title">VISITA</h2>
        <p class="card-text">📍 Colón n.11, Centro, Tlaxiaco, Oaxaca</p>
        <a href="#" class="btn btn-primary">VISITAR</a>
      </div>
    </div>

    <!-- Botón regresar -->
    <div class="mt-4 text-start">
      <a href="#" class="btn btn-outline-secondary">⬅️ REGRESAR</a>
    </div>
  </div>
</template>

<script setup>
// No hay lógica compleja, solo template
</script>

<style scoped>
.logo {
  max-width: 150px;
}
.card img {
  max-height: 1000px;
  object-fit: cover;
}
</style>
