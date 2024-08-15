<template>
  <div class="d-flex flex-column min-vh-100">
    <!-- Header -->
    <nav v-if="!isLoginPage" class="d-flex justify-content-between align-items-center p-3" style="background: linear-gradient(to bottom, #3a7d56, #024716);">
      <div class="d-flex align-items-center">
        <img 
          src="@/assets/menuburger.png" 
          alt="Logo" 
          class="img-fluid" 
          style="max-height: 40px; cursor: pointer;" 
          @click="toggleSidebar" 
        />
      </div>
      <div class="d-flex align-items-center">
        <ul class="nav">
          <li class="nav-item">
            <router-link to="/" class="nav-link text-white mx-3">Inicio</router-link>
          </li>
          <li class="nav-item">
            <router-link to="/programslist" class="nav-link text-white mx-3">Lista de Programas</router-link>
          </li>
          <li class="nav-item">
            <router-link to="/plansandpricing" class="nav-link text-white mx-3">Planes y Precios</router-link>
          </li>
          <li class="nav-item">
            <router-link to="/contactus" class="nav-link text-white mx-3">Contáctanos</router-link>
          </li>
        </ul>
        <span class="user-name" style="background-color: rgba(255, 255, 255, 0.1); border-radius: 15px; padding: 5px 10px; color: white; margin-left: 10px; margin-right: 5px; pointer-events: none;">
          Juan Perez
        </span>
        <img src="@/assets/login-icon.svg" alt="Perfil" class="rounded-circle" style="height: 40px;">
      </div>
    </nav>

    <!-- Sidebar -->
    <aside v-if="!isLoginPage" :class="{'sidebar-open': sidebarOpen, 'sidebar-close': !sidebarOpen}" class="sidebar d-flex flex-column">
      <div class="p-4 text-center">
        <img 
          src="@/assets/logo-principal.png" 
          alt="Logo" 
          class="img-fluid mb-4" 
          style="max-height: 80px; cursor: pointer;" 
          @click="closeSidebar" 
        />
        <ul class="list-unstyled">
          <li><router-link to="/" class="sidebar-link">Dashboard</router-link></li>
          <li><router-link to="/profile" class="sidebar-link">Perfil</router-link></li>
          <li><router-link to="/courses" class="sidebar-link">Cursos</router-link></li>
          <li><router-link to="/schedule" class="sidebar-link">Horario de clases</router-link></li>
          <li><router-link to="/calendar" class="sidebar-link">Calendario</router-link></li>
          <li><router-link to="/grades" class="sidebar-link">Calificaciones</router-link></li>
          <li><router-link to="/liveclasses" class="sidebar-link">Clases en Vivo</router-link></li>
        </ul>
      </div>
      <div class="flex-grow-1"></div>
      <div class="p-4">
        <router-link to="/login" class="sidebar-link logout-link">Cerrar Sesión</router-link>
      </div>
    </aside>

    <!-- Contenido Principal -->
    <main class="flex-grow-1 p-5 bg-white" :class="{'content-shifted': sidebarOpen}" v-if="!isLoginPage">
      <RouterView />
    </main>

    <!-- Footer -->
    <footer v-if="!isLoginPage" class="text-center p-2" style="background-color: white; border-top: 2px solid #55bf84; color: #024716;">
      <p class="mb-0">© 2024 Aprende Sin Límites. Todos los derechos reservados.</p>
    </footer>

    <!-- Contenido del Login -->
    <div v-if="isLoginPage" class="full-screen-login">
      <RouterView />
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      sidebarOpen: false,
    };
  },
  computed: {
    isLoginPage() {
      return this.$route.path === '/login'; // Asegúrate de que la ruta sea la correcta
    },
  },
  methods: {
    toggleSidebar() {
      this.sidebarOpen = !this.sidebarOpen;
    },
    closeSidebar() {
      this.sidebarOpen = false;
    },
  },
};
</script>

<style>
/* Estilos generales y del layout */
html, body {
  height: 100%;
}

.sidebar {
  background-color: #3a7d56;
  width: 250px;
  position: fixed;
  top: 0;
  bottom: 0;
  left: -250px;
  transition: left 0.3s ease;
  z-index: 1000;
}

.sidebar-open {
  left: 0;
}

.content-shifted {
  margin-left: 250px;
}

.sidebar-link {
  color: white;
  text-decoration: none;
  display: block;
  padding: 10px 15px;
  transition: background 0.3s;
}

.sidebar-link:hover {
  background-color: rgba(255, 255, 255, 0.1);
  border-radius: 5px;
}

.logout-link {
  color: #cc0000;
  text-align: center;
  display: block;
}

.logout-link:hover {
  color: #990000;
}

/* Estilo para la vista de login */
.full-screen-login {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh; /* Ocupa toda la altura de la pantalla */
  background-color: #55bf84; /* Color de fondo de la vista de login */
}
</style>

