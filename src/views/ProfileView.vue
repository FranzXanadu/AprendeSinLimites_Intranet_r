<template>
    <div class="perfil">
      <h2 class="mb-4" style="color: #024716;">Perfil del Usuario</h2>
  
      <!-- Información Personal -->
      <div class="card shadow-sm mb-4">
        <div class="card-body">
          <h5 class="card-title" style="color: #55bf84;">Información Personal</h5>
          <p style="color: #024716;">Nombre: Juan Perez</p>
          <p style="color: #024716;">Correo Electrónico: juan.perez@correo.com</p>
          <p style="color: #024716;">Teléfono: (123) 456-7890</p>
        </div>
      </div>
  
      <!-- Configuración de Cuenta -->
      <div class="card shadow-sm mb-4">
        <div class="card-body">
          <h5 class="card-title" style="color: #55bf84;">Configuración de Cuenta</h5>
          <p style="color: #024716;">Cambiar Contraseña</p>
          <p style="color: #024716;">Configuración de Privacidad</p>
        </div>
      </div>
  
      <!-- Progreso del Usuario -->
      <div class="card shadow-sm mb-4">
        <div class="card-body">
          <h5 class="card-title" style="color: #55bf84;">Progreso del Usuario</h5>
          <div class="progress mb-3">
            <div
              class="progress-bar"
              role="progressbar"
              style="width: 75%; background-color: #55bf84;"
              aria-valuenow="75"
              aria-valuemin="0"
              aria-valuemax="100"
            >
              75% Completo
            </div>
          </div>
        </div>
      </div>
  
      <!-- Actividad Reciente -->
      <div class="card shadow-sm mb-4">
        <div class="card-body">
          <h5 class="card-title" style="color: #55bf84;">Actividad Reciente</h5>
          <ul class="list-unstyled">
            <li class="mb-3">
              <h6 style="color: #024716;">Completado: Curso de Literatura</h6>
              <p class="text-secondary">Fecha: 10 de agosto, 2024</p>
            </li>
            
            <li class="mb-3">
              <h6 style="color: #024716;">Actualización de Perfil</h6>
              <p class="text-secondary">Fecha: 1 de agosto, 2024</p>
            </li>

            <li class="mb-3">
              <h6 style="color: #024716;">Inscripción en: Ciclo Virtual</h6>
              <p class="text-secondary">Fecha: 5 de abril, 2024</p>
            </li>
          </ul>
        </div>
      </div>
  
      <!-- Botón para Editar Perfil -->
      <div class="d-flex justify-content-center">
        <button
          class="btn btn-gradient text-white fw-semibold shadow-sm"
          style="background-color: #024716;"
        >
          Editar Perfil
        </button>
      </div>
    </div>
  </template>
  