<template>
    <div class="contact-us">
      <h2 class="mb-4" style="color: #024716;">Contáctanos</h2>
  
      <div class="container">
        <div class="row">
          <div class="col-md-6">
            <h5 style="color: #55bf84;">¡Únete a nuestro equipo!</h5>
            <p>
              Estamos en busca de profesores apasionados y comprometidos con la educación. Si deseas formar parte de nuestro equipo, por favor completa el siguiente formulario y nos pondremos en contacto contigo.
            </p>
            <form>
              <div class="mb-3">
                <label for="name" class="form-label">Nombre completo</label>
                <input type="text" class="form-control" id="name" required>
              </div>
              <div class="mb-3">
                <label for="email" class="form-label">Correo electrónico</label>
                <input type="email" class="form-control" id="email" required>
              </div>
              <div class="mb-3">
                <label for="subject" class="form-label">Materia que deseas enseñar</label>
                <input type="text" class="form-control" id="subject" required>
              </div>
              <div class="mb-3">
                <label for="message" class="form-label">Mensaje</label>
                <textarea class="form-control" id="message" rows="4" required></textarea>
              </div>
              <button type="submit" class="btn btn-success">Enviar</button>
            </form>
          </div>
  
          <div class="col-md-6">
            <h5 style="color: #55bf84;">Información de contacto</h5>
            <p>Si prefieres contactarnos directamente, aquí tienes nuestra información:</p>
            <p><strong>Teléfono:</strong> 123-456-789</p>
            <p><strong>Correo electrónico:</strong> info@academia.com</p>
            <p><strong>Dirección:</strong> Av. Ejemplo 123, Ciudad</p>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <style scoped>
  .contact-us {
    padding: 20px;
  }
  
  h5 {
    margin-top: 20px;
  }
  
  .btn-success {
    background-color: #55bf84;
    border-color: #55bf84;
  }
  
  .btn-success:hover {
    background-color: #024716;
    border-color: #024716;
  }
  </style>
  