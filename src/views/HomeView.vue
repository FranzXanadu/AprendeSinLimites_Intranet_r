<template>

  <!-- Contenido Principal -->
  
  <div class="dashboard">
    <h2 class="mb-4" style="color: #024716;">Dashboard</h2>

    <!-- Estadísticas -->
    <div class="row mb-4">
      <div class="col-md-3">
        <div class="card text-center shadow-sm">
          <div class="card-body">
            <h5 class="card-title" style="color: #55bf84;">Total de Cursos</h5>
            <p class="card-text" style="font-size: 24px; color: #024716;">6</p>
          </div>
        </div>
      </div>
      <div class="col-md-3">
        <div class="card text-center shadow-sm">
          <div class="card-body">
            <h5 class="card-title" style="color: #55bf84;">Estudiantes Inscritos</h5>
            <p class="card-text" style="font-size: 24px; color: #024716;">150</p>
          </div>
        </div>
      </div>
      <div class="col-md-3">
        <div class="card text-center shadow-sm">
          <div class="card-body">
            <h5 class="card-title" style="color: #55bf84;">Tasa de Éxito</h5>
            <p class="card-text" style="font-size: 24px; color: #024716;">85%</p>
          </div>
        </div>
      </div>
      <div class="col-md-3">
        <div class="card text-center shadow-sm">
          <div class="card-body">
            <h5 class="card-title" style="color: #55bf84;">Nuevos Inscritos</h5>
            <p class="card-text" style="font-size: 24px; color: #024716;">12</p>
          </div>
        </div>
      </div>
    </div>

    <!-- Gráficos (simulados) -->
    <div class="card shadow-sm mb-4">
      <div class="card-body">
        <h5 class="card-title" style="color: #024716;">Avance de Tareas</h5>
        <div class="mb-3">
          <h6>Curso: Matemáticas</h6>
          <div class="progress">
            <div class="progress-bar" role="progressbar" style="width: 70%; background-color: #55bf84;" aria-valuenow="70" aria-valuemin="0" aria-valuemax="100">70%</div>
          </div>
        </div>
        <div class="mb-3">
          <h6>Curso: Biología</h6>
          <div class="progress">
            <div class="progress-bar" role="progressbar" style="width: 50%; background-color: #55bf84;" aria-valuenow="50" aria-valuemin="0" aria-valuemax="100">50%</div>
          </div>
        </div>
        <div class="mb-3">
          <h6>Curso: Historia Universal</h6>
          <div class="progress">
            <div class="progress-bar" role="progressbar" style="width: 90%; background-color: #55bf84;" aria-valuenow="90" aria-valuemin="0" aria-valuemax="100">90%</div>
          </div>
        </div>
        <div class="mb-3">
          <h6>Curso: Trigonometría</h6>
          <div class="progress">
            <div class="progress-bar" role="progressbar" style="width: 30%; background-color: #55bf84;" aria-valuenow="30" aria-valuemin="0" aria-valuemax="100">30%</div>
          </div>
        </div>
      </div>
    </div>

    <!-- Sección de Noticias -->
    <div class="card shadow-sm mb-4">
      <div class="card-body">
        <h5 class="card-title" style="color: #024716;">Noticias Recientes</h5>
        <ul class="list-unstyled">
          <li class="mb-3">
            <h6 style="color: #024716;">Nuevos Cursos Disponibles</h6>
            <p class="text-secondary">Las inscripciones para los nuevos cursos de matemáticas y biología están abiertas hasta el 30 de septiembre.</p>
          </li>
          <li class="mb-3">
            <h6 style="color: #024716;">Conferencia sobre Estrategias de Aprendizaje</h6>
            <p class="text-secondary">Únete a nosotros el 22 de agosto para una conferencia sobre técnicas efectivas de estudio.</p>
          </li>
          <li class="mb-3">
            <h6 style="color: #024716;">Resultados del Último Examen</h6>
            <p class="text-secondary">Los resultados del examen de fin de curso se publicarán el 29 de agosto en la plataforma.</p>
          </li>
          <li class="mb-3">
            <h6 style="color: #024716;">Actualización del Plan de Estudios</h6>
            <p class="text-secondary">El nuevo plan de estudios para el próximo semestre se anunciará el 1 de septiembre.</p>
          </li>
        </ul>
      </div>
    </div>

    <!-- Listado de Cursos -->
    <div class="card shadow-sm mb-4">
      <div class="card-body">
        <h5 class="card-title" style="color: #024716;">Cursos Ofrecidos</h5>
        <ul class="list-group">
          <li class="list-group-item">Matemáticas</li>
          <li class="list-group-item">Biología</li>
          <li class="list-group-item">Historia Universal</li>
          <li class="list-group-item">Historia del Perú</li>
          <li class="list-group-item">Trigonometría</li>
          <li class="list-group-item">Literatura</li>
        </ul>
      </div>
    </div>
  </div>

</template>

<style scoped>
.dashboard {
  padding: 20px;
}
</style>

<!-- <style>
html, body {
  height: 100%; /* Asegura que el cuerpo y el HTML ocupen toda la altura */
}

.footer {
  margin-top: auto; /* Esto empuja el footer hacia abajo */
}
.dashboard {
  padding: 20px;
}

.card-title {
  color: #024716; /* Color del título de la tarjeta */
}
.sidebar {
  background-color: #3a7d56;
  width: 250px;
  position: fixed;
  top: 0;
  bottom: 0;
  left: -250px; /* Oculta la barra lateral inicialmente */
  transition: left 0.3s ease; /* Animación al abrir/cerrar */
  z-index: 1000;
}

.sidebar-open {
  left: 0; /* Muestra la barra lateral cuando está abierta */
}

.content-shifted {
  margin-left: 250px; /* Desplaza el contenido principal hacia la derecha cuando el sidebar está abierto */
}

.btn-gradient {
  background: linear-gradient(to bottom, #3a7d56, #024716);
  color: white; /* Cambia el color del texto según sea necesario */
  border: none; /* Asegúrate de que no haya borde si no lo deseas */
}

.btn-gradient:hover {
  background: linear-gradient(to bottom, #2a5d46, #024716); /* Color en hover (opcional) */
}

/* Estilos para los enlaces en el menú hamburguesa */
.sidebar-link {
  color: white; /* Color del texto */
  text-decoration: none; /* Elimina el subrayado */
  display: block; /* Para que toda el área del enlace sea clickable */
  padding: 10px 15px; /* Espaciado interno */
  transition: background 0.3s; /* Suaviza el cambio de fondo */
}

.sidebar-link:hover {
  background-color: rgba(255, 255, 255, 0.1); /* Color de fondo al pasar el mouse (opcional) */
  border-radius: 5px; /* Bordes redondeados (opcional) */
}

/* Estilos específicos para el enlace de cerrar sesión */
.logout-link {
  color: #cc0000; /* Color de texto rojo más oscuro */
  padding: 10px 15px; /* Espaciado interno */
  border-radius: 5px; /* Bordes redondeados */
  text-align: center; /* Centra el texto */
  display: block; /* Para que el enlace ocupe todo el ancho */
  transition: color 0.3s; /* Suaviza el cambio de color */
}

.logout-link:hover {
  color: #990000; /* Color de texto más oscuro al pasar el mouse */
}
</style>

<script>
export default {
  data() {
    return {
      sidebarOpen: false, // Controla el estado del menú hamburguesa
    };
  },
  methods: {
    toggleSidebar() {
      this.sidebarOpen = !this.sidebarOpen; // Alterna el estado del menú hamburguesa
    },
    closeSidebar() {
      this.sidebarOpen = false; // Cierra el menú hamburguesa
    },
  },
};
</script> -->
