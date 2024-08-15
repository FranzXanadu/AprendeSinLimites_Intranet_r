<template>
  <div class="live-classes-view">
    <h2 class="mb-4" style="color: #024716;">Clases en Vivo</h2>

    <div class="card shadow-sm mb-4">
      <div class="card-body">
        <h5 class="card-title" style="color: #55bf84;">Detalles de la Próxima Clase</h5>
        <div class="class-info mb-3">
          <div class="row">
            <div class="col-md-6">
              <h6><strong>Asignatura:</strong></h6>
              <p>Biología</p>
            </div>
            <div class="col-md-6">
              <h6><strong>Fecha:</strong></h6>
              <p>Lunes, 18 de agosto</p>
            </div>
            <div class="col-md-6">
              <h6><strong>Hora:</strong></h6>
              <p>8:00 AM - 9:00 AM</p>
            </div>
            <div class="col-md-6">
              <h6><strong>Enlace para Unirse:</strong></h6>
              <a href="#" class="btn btn-success">Unirse a la Clase</a>
            </div>
          </div>
        </div>

        <div class="class-description mb-3">
          <h6><strong>Descripción:</strong></h6>
          <p>En esta clase exploraremos los conceptos fundamentales de Biología, incluyendo la célula, la genética y la evolución. Prepárate para una sesión interactiva con ejemplos prácticos.</p>
        </div>

        <div class="class-resources mb-3">
          <h6><strong>Recursos Recomendados:</strong></h6>
          <ul>
            <li><a href="#">Lectura: Introducción a la Biología</a></li>
            <li><a href="#">Video: Conceptos Básicos de Genética</a></li>
            <li><a href="#">Documento: Guía de Estudio de Biología</a></li>
          </ul>
        </div>

        <div class="alert alert-info mt-3">
          <strong>Nota:</strong> Asegúrate de revisar los materiales recomendados antes de la clase y de tener una buena conexión a Internet.
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.live-classes-view {
  padding: 20px;
}

.class-info {
  border-bottom: 1px solid #ddd;
  padding-bottom: 15px;
}

.class-info h6 {
  margin-bottom: 5px;
}

.class-description, .class-resources {
  border-bottom: 1px solid #ddd;
  padding-bottom: 15px;
}

.class-description p, .class-resources ul {
  margin-bottom: 15px;
}

.class-resources ul {
  list-style-type: none;
  padding-left: 0;
}

.class-resources li {
  margin-bottom: 5px;
}

.class-resources a {
  color: #55bf84;
  text-decoration: none;
}

.class-resources a:hover {
  text-decoration: underline;
}
</style>
