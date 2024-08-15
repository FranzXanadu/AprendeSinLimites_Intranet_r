<template>
    <body class="d-flex justify-content-center align-items-center vh-100" style="background-color: #55bf84;">
    <div
      class="bg-white p-5 rounded-5 text-secondary shadow"
      style="width: 25rem"
    >
      <div class="d-flex justify-content-center">
        <img
          src="@/assets/logo-aprendersinlimites-letras.png"
          alt="login-icon"
          style="height: 14rem"
        />
      </div>
      <!-- <div class="text-center fs-1 fw-bold">Login</div> -->
      <div class="input-group mt-4">
        <div class="input-group-text" style="background-color: #024716;">
          <img
            src="@/assets/username-icon.svg"
            alt="username-icon"
            style="height: 1rem"
          />
        </div>
        <input
          class="form-control bg-light"
          type="text"
          placeholder="Usuario"
        />
      </div>
      <div class="input-group mt-1">
        <div class="input-group-text" style="background-color: #024716;">
          <img
            src="@/assets/password-icon.svg"
            alt="password-icon"
            style="height: 1rem"
          />
        </div>
        <input
          class="form-control bg-light"
          type="password"
          placeholder="Contraseña"
        />
      </div>
      <div class="d-flex justify-content-around mt-1">
        <div class="d-flex align-items-center gap-1">
          <input class="form-check-input" type="checkbox" />
          <div class="pt-1" style="font-size: 0.9rem">Recuerdame</div>
        </div>
        <div class="pt-1">
          <a
            href="#"
            class="text-decoration-none text-success fw-semibold fst-italic"
            style="font-size: 0.9rem"
            >Olvidaste tu contraseña?</a
          >
        </div>
      </div>
      <router-link to="/">
        <div class="btn btn-gradient text-white w-100 mt-4 fw-semibold shadow-sm" style="background-color: #024716;">
          Ingresar
        </div>
      </router-link>
      <div class="d-flex gap-1 justify-content-center mt-1">
        <div>No tiene una cuenta?</div>
        <a href="#" class="text-decoration-none text-success fw-semibold"
          >Registrar</a
        >
      </div>
      <div class="p-3">
        <div class="border-bottom text-center" style="height: 0.9rem">
          <span class="bg-white px-3">o</span>
        </div>
      </div>
      <div
        class="btn btn-white-custom d-flex gap-2 justify-content-center border mt-3 shadow-sm"
      >
        <img
          src="@/assets/google-icon.svg"
          alt="google-icon"
          style="height: 1.6rem"
        />
        <div class="fw-semibold text-secondary">Continuar con Google</div>
      </div>
    </div>
  </body>
</template>

<style>
.btn-gradient {
  background: linear-gradient(to bottom, #3a7d56, #024716);
  color: white; /* Cambia el color del texto según sea necesario */
  border: none; /* Asegúrate de que no haya borde si no lo deseas */
}

.btn-gradient:hover {
  background: linear-gradient(to bottom, #2a5d46, #024716); /* Color en hover (opcional) */
}

input.form-control:focus {
  border-color: #55bf84; /* Cambia el color del borde al hacer foco */
  box-shadow: 0 0 0 0.2rem rgba(85, 191, 132, 0.25); /* Cambia el color del sombreado al hacer foco */
  background-color: #e6f5ee; /* (Opcional) Cambia el color de fondo cuando está en foco */
}
input.form-check-input:focus {
  border-color: #55bf84; /* Cambia el color del borde al hacer foco */
  box-shadow: 0 0 0 0.2rem rgba(85, 191, 132, 0.25); /* Cambia el color del sombreado al hacer foco */
}
</style>