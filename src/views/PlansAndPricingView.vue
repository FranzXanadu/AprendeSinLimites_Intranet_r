<template>
    <div class="price-list">
      <h2 class="mb-4" style="color: #024716;">Lista de Precios</h2>
  
      <div class="container">
        <div class="row">
          <!-- Ciclo Virtual -->
          <div class="col-md-4 mb-4">
            <div class="card shadow-sm border-success card-height">
              <div class="card-body text-center">
                <h5 class="card-title">Ciclo Virtual</h5>
                <p class="card-price">S/800.00</p>
                <p>Incluye:</p>
                <ul class="text-left">
                  <li>Clases en vivo</li>
                  <li>Clases grabadas en HD</li>
                  <li>Simulacros tipo admisión</li>
                  <li>Foro de dudas</li>
                </ul>
                <a href="#" class="btn btn-success">Comprar</a>
              </div>
            </div>
          </div>
  
          <!-- Verano/Repaso -->
          <div class="col-md-4 mb-4">
            <div class="card shadow-sm border-success card-height">
              <div class="card-body text-center">
                <h5 class="card-title">Verano/Repaso</h5>
                <p class="card-price">S/300.00</p>
                <p>Incluye:</p>
                <ul class="text-left">
                  <li>Clases virtuales</li>
                  <li>Materiales de estudio</li>
                  <li>Simulacros tipo admisión</li>
                  <li>Foro de dudas</li>
                </ul>
                <a href="#" class="btn btn-success">Comprar</a>
              </div>
            </div>
          </div>
  
          <!-- Precio por Curso (Ciclo) -->
          <div class="col-md-4 mb-4">
            <div class="card shadow-sm border-success card-height">
              <div class="card-body text-center">
                <h5 class="card-title">Precio por Curso (Ciclo)</h5>
                <p class="card-price">S/80.00</p>
                <p>Incluye:</p>
                <ul class="text-left">
                  <li>Acceso a las clases virtuales</li>
                  <li>Materiales de estudio</li>
                </ul>
                <a href="#" class="btn btn-success">Comprar</a>
              </div>
            </div>
          </div>
  
          <!-- Precio por Curso (Verano/Repaso) -->
          <div class="col-md-4 mb-4">
            <div class="card shadow-sm border-success card-height">
              <div class="card-body text-center">
                <h5 class="card-title">Precio por Curso (Verano/Repaso)</h5>
                <p class="card-price">S/30.00</p>
                <p>Incluye:</p>
                <ul class="text-left">
                  <li>Acceso a las clases virtuales</li>
                  <li>Materiales de estudio</li>
                </ul>
                <a href="#" class="btn btn-success">Comprar</a>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <style scoped>
  .price-list {
    padding: 20px;
  }
  
  .card {
    background-color: #f9f9f9;
    border: 2px solid #55bf84; /* Borde verde */
    border-radius: 10px;
    transition: transform 0.2s;
  }
  
  .card:hover {
    transform: scale(1.05); /* Efecto de escalado */
  }
  
  .card-title {
    color: #024716;
    font-weight: bold;
  }
  
  .card-price {
    font-size: 1.5rem;
    color: #55bf84;
    font-weight: bold;
  }
  
  .btn-success {
    background-color: #55bf84;
    border-color: #55bf84;
  }
  
  .btn-success:hover {
    background-color: #024716;
    border-color: #024716;
  }
  
  .text-left {
    text-align: left;
  }
  
  .card-height {
    height: 400px; /* Altura fija para los cards */
  }
  </style>
  