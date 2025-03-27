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

  
<!-- Título -->
<h1 class="text-center mt-4">EL PATIO</h1>
    <div class="text-center">
      <span class="badge bg-warning text-dark">✨</span>
      <span class="badge bg-warning text-dark">✨</span>
    </div>

    <!-- Imagen con descripción -->
    <div class="card mt-4">
      <img src="/patio.jpg" class="img-fluid" alt="El patio" />
      <div class="card-body text-center">
        <h2 class="card-title">VISITA</h2>
        <p class="card-text">📍 Isabel la Católica N.4, San Sebastian, Tlaxiaco, Oaxaca</p>
        <a href="#" class="btn btn-primary">VISITAR</a>
      </div>
    </div>

 
    <!-- Título -->
    <h1 class="text-center mt-4">LA MESA DEL RINCÓN</h1>
    <div class="text-center">
      <span class="badge bg-warning text-dark">✨</span>
      <span class="badge bg-warning text-dark">✨</span>
    </div>

    <!-- Imagen con descripción -->
    <div class="card mt-4">
      <img src="/mesa.png" class="img-fluid" alt="Mesa del Rincón" />
      <div class="card-body text-center">
        <h2 class="card-title">VISITA</h2>
        <p class="card-text">📍 Paseo de la Reforma N.16, Col. Benito Juarez, Tlaxiaco, Oaxaca</p>
        <a href="#" class="btn btn-primary">VISITAR</a>
      </div>
    </div>

 
    <!-- Título -->
    <h1 class="text-center mt-4">TLAYUDAS EL NEGRO</h1>
    <div class="text-center">
      <span class="badge bg-warning text-dark">✨</span>
      <span class="badge bg-warning text-dark">✨</span>
    </div>

    <!-- Imagen con descripción -->
    <div class="card mt-4">
      <img src="/tlayudas.png" class="img-fluid" alt="Tlayudas el Negro" />
      <div class="card-body text-center">
        <h2 class="card-title">VISITA</h2>
        <p class="card-text">📍 Hipodromo N.8, Centro, Tlaxiaco, Oaxaca</p>
        <a href="#" class="btn btn-primary">VISITAR</a>
      </div>
    </div>

     </div>
</template>

<style scoped>
.logo {
  max-width: 150px;
}
.card img {
  max-height: 1000px;
  object-fit: cover;
}
</style>
