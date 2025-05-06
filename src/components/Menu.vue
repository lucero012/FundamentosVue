<template>
    <div class="container mt-5">
  
      <!-- Encabezado con logo, búsqueda y carrito -->
      <div class="d-flex justify-content-between align-items-center">
        <!-- Logo -->
        <img src="/logo.png" alt="Logo WebFood" class="logo img-fluid" style="max-height: 90px;">
        
        <!-- Barra de búsqueda -->
        <div class="input-group w-50">
          <span class="input-group-text">🔍</span>
          <input type="text" class="form-control" placeholder="BUSCAR PRODUCTO" />
        </div>
  
        <!-- Ícono del carrito -->
        <img src="/carro.jpeg" alt="Carrito de compras" class="cart-icon img-fluid" style="max-height: 50px;">
      </div>
  
      <!-- Título del menú -->
      <h1 class="text-center mt-4">MENÚ</h1>
  
      <!-- Tabla del menú -->
      <div class="table-responsive mt-4">
        <table class="table table-hover table-striped table-bordered">
          <thead class="table-dark">
            <tr>
              <th class="text-center">#</th>
              <th class="text-center">Opciones</th>
              <th class="text-center">Navegar</th>
            </tr>
          </thead>
          <tbody>
            <tr v-for="(item, index) in menu" :key="item.id">
              <td class="text-center">{{ index + 1 }}</td>
              <td class="text-center">{{ item.nombre }}</td>
              <td class="text-center">
                <button 
                  class="btn btn-primary btn-sm"
                  @click="seleccionarOpcion(item.nombre)"
                >
                  Ver
                </button>
              </td>
            </tr>
          </tbody>
        </table>
      </div>
  
    </div>
  </template>
  
<script setup>
import { ref } from 'vue';

// Datos del menú
const menu = ref([
  { id: 1, nombre: "BEBIDAS" },
  { id: 2, nombre: "COMIDAS" },
  { id: 3, nombre: "BOTANAS" },
  { id: 4, nombre: "POSTRES" }
]);


</script>
  