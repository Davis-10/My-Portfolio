<template>
    <aside class="sidebar">
      <!-- Parte superior: imagen y descripción -->
      <div class="sidebar-top">
           
            <h1>David Bustos</h1>
            <p class="role">Desarrollador Frontend</p>
            <p class="bio">
            ¡Hola! Soy un apasionado desarrollador frontend con experiencia en Vue.js y un enfoque en la
            creación de aplicaciones web atractivas y funcionales.
            </p>
            <p class="bio">
            Me encanta aprender y mejorar mis habilidades constantemente.
            </p>
            <p class="bio">
            ¡Estoy emocionado por el futuro y las oportunidades que me esperan!
            </p>
            <img src="@/assets/image-david.png" alt="Imagen David" class="logo" />
      </div>
  
      <!-- Menú de navegación -->
      <nav class="sidebar-nav">
        <ul>
          <li><RouterLink to="/">Home</RouterLink></li>
          <li><RouterLink to="/about">About</RouterLink></li>
          <li><RouterLink to="/experience">Experience</RouterLink></li>
          <li><RouterLink to="/projects">Projects</RouterLink></li>
          <li><RouterLink to="/contact">Contact</RouterLink></li>
        </ul>
      </nav>
  
      <!-- Footer con iconos sociales -->
      <div class="sidebar-footer">
        <a href="https://www.linkedin.com/in/david-bustos-b46b6911a/" target="_blank" rel="noopener" aria-label="LinkedIn">
          <font-awesome-icon :icon="['fab', 'linkedin']" />
        </a>
        <a href="https://github.com/Davis-10" target="_blank" rel="noopener" aria-label="GitHub">
          <font-awesome-icon :icon="['fab', 'github']" />
        </a>
        <a href="https://www.instagram.com/bustosdavid10" target="_blank" rel="noopener" aria-label="Instagram">
          <font-awesome-icon :icon="['fab', 'instagram']" />
        </a>
      </div>
    </aside>
  </template>
  
  
  <style scoped>
  .sidebar {
    margin-left: 100px;
    width: 600px;
    height: 100vh;
    color: #ccd6f6;
    display: flex; 
    justify-content: center; /* Centrado horizontal */
    align-items: center; /* Centrado vertical */
  }
  
  /* Parte superior */
.sidebar-top {
  text-align: center;
  margin-bottom: 20px;
}

.logo {
  width: 300px;
  height: 400px;
  border-radius: 50%;
  object-fit: cover;
  margin-top: 50px;
  border: 3px solid #64ffda;
}

h1 {
  font-size: 2.5rem;
  margin-bottom: 5px;
  color: #64ffda;
  font-weight: 700;
}

.role {
  font-size: 1.4rem;
  font-weight: 500;
  margin-bottom: 30px;
  color: #8892b0;
}

.bio {
  font-size: 1.2rem;
  line-height: 1.4;
  margin-bottom: 20px;
  color: #a8b2d1;
}

/* Navegación */
.sidebar-nav ul {
  list-style: none;
  padding: 0;
  margin: 0 80px 0 60px;
}

.sidebar-nav li {
  margin-bottom: 18px;
}

.sidebar-nav a {
  font-size: 1.3rem;
  color: #64ffda;
  text-decoration: none;
  font-weight: 600;
  transition: color 0.3s ease;
}

.sidebar-nav a.router-link-exact-active,
.sidebar-nav a:hover {
  color: #a0eaff;
}

/* Footer social */
.sidebar-footer {
  display: flex;
  justify-content: center;
  gap: 30px;
  padding-top: 10px;
  border-top: 1px solid #233554;
}

.sidebar-footer a {
  color: #64ffda;
  font-size: 2rem;
  transition: color 0.3s ease;
}

.sidebar-footer a:hover {
  color: #a0eaff;
}
  </style>
  