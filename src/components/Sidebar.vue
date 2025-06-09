<template>
  <aside class="sidebar">
    <div class="sidebar-content">
      <!-- Parte superior: imagen y descripción -->
      <div class="sidebar-top">
        <!-- Imagen de perfil mejorada con borde y posición -->
        <div class="profile-image-container">
          <div class="profile-image">
            <img src="@/assets/image-david.png" alt="Imagen David" class="logo" />
          </div>
        </div>
        
        <div class="profile-info">
          <h1>David Bustos</h1>
          <p class="role">Desarrollador Web FullStack</p>
        </div>
        
        <div class="bio-container">
          <p class="bio">
            ¡Hola! Soy un apasionado desarrollador web FullStack con experiencia en HTML5, CSS3, JavaScript, Vue.js, Python y un enfoque en la
            creación de aplicaciones web atractivas y funcionales. Me encanta aprender y mejorar mis habilidades constantemente.
          </p>
      
          <p class="bio">
            ¡Estoy emocionado por el futuro y las oportunidades que me esperan!
          </p>
        </div>
      </div>

      <!-- Contenedor para nav y footer -->
      <div class="nav-footer-container">
        <!-- Menú de navegación -->
        <nav class="sidebar-nav">
          <ul>
            <li><RouterLink to="/" class="nav-link">Home</RouterLink></li>
            <li><RouterLink to="/about" class="nav-link">About</RouterLink></li>
            <li><RouterLink to="/experience" class="nav-link">Experience</RouterLink></li>
            <li><RouterLink to="/projects" class="nav-link">Projects</RouterLink></li>
            <li><RouterLink to="/contact" class="nav-link">Contact</RouterLink></li>
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
          <!-- <a href="https://www.instagram.com/bustosdavid10" target="_blank" rel="noopener" aria-label="Instagram">
            <font-awesome-icon :icon="['fab', 'instagram']" />
          </a> -->
        </div>
      </div>
    </div>
  </aside>
</template>

<script setup>
import { onMounted, onUnmounted } from 'vue';

// Función para actualizar el enlace activo según el scroll
const handleScroll = () => {
  const sections = document.querySelectorAll('section[id]');
  const navLinks = document.querySelectorAll('.nav-link');
  
  let currentSection = '';
  
  sections.forEach(section => {
    const sectionTop = section.offsetTop;
    const sectionHeight = section.offsetHeight;
    
    if (window.scrollY >= sectionTop - 100 && 
        window.scrollY < sectionTop + sectionHeight - 100) {
      currentSection = section.getAttribute('id');
    }
  });
  
  navLinks.forEach(link => {
    link.classList.remove('active-section');
    
    // Extraer el id de sección del href
    const href = link.getAttribute('href');
    const linkPath = href.split('/').filter(Boolean)[0] || 'home';
    
    if (currentSection === linkPath || 
        (currentSection === '' && linkPath === 'home')) {
      link.classList.add('active-section');
    }
  });
};

// Agregar y remover el event listener para el scroll
onMounted(() => {
  window.addEventListener('scroll', handleScroll);
  // Llamar una vez al cargar para establecer el estado inicial
  handleScroll();
});

onUnmounted(() => {
  window.removeEventListener('scroll', handleScroll);
});
</script>

<style scoped>
/* Fuente monoespaciada para todo el componente */
:root {
  font-family: 'SF Mono', 'Fira Code', 'JetBrains Mono', 'Roboto Mono', monospace;
}

.sidebar {
  width: 350px;
  height: 100vh;
  padding: 40px 20px;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  position: sticky;
  top: 0;
  left: 0;
  color: #ccd6f6;
  border-right: 1px solid #233554;
}

.sidebar-content {
  display: flex;
  flex-direction: column;
  height: 100%;
}

/* Parte superior */
.sidebar-top {
  text-align: left;
  margin-bottom: 30px;
}

/* Contenedor de imagen mejorado */
.profile-image-container {
  display: flex;
  justify-content: center;
  margin-bottom: 30px;
  position: relative;
}

.profile-image {
  width: 200px;
  height: 200px;
  border-radius: 10px;
  overflow: hidden;
  border: 3px solid #64ffda;
  box-shadow: 0 10px 30px rgba(100, 255, 218, 0.2);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  position: relative;
}

.profile-image:hover {
  transform: translateY(-5px);
  box-shadow: 0 15px 30px rgba(100, 255, 218, 0.3);
}

.profile-image::after {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: rgba(100, 255, 218, 0.1);
  border-radius: 10px;
  opacity: 0;
  transition: opacity 0.3s ease;
}

.profile-image:hover::after {
  opacity: 1;
}

.logo {
  width: 100%;
  height: 100%;
  object-fit: cover;
  object-position: center top;
}

.profile-info {
  margin-bottom: 20px;
}

h1 {
  font-size: 2.2rem;
  margin-bottom: 5px;
  color: #64ffda;
  font-weight: 700;
}

.role {
  font-size: 1.1rem;
  font-weight: 500;
  color: #8892b0;
}

.bio-container {
  margin-top: 20px;
}

.bio {
  font-size: 0.95rem;
  line-height: 1.5;
  margin-bottom: 15px;
  color: #a8b2d1;
}

/* Contenedor para nav y footer */
.nav-footer-container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 30px;
  margin-top: 3rem;
}

/* Navegación */
.sidebar-nav {
  flex: 1;
}

.sidebar-nav ul {
  list-style: none;
  padding: 0;
  margin: 0;
}

.sidebar-nav li {
  margin-bottom: 12px;
  position: relative;
}

.nav-link {
  font-size: 1.1rem;
  color: #8892b0;
  text-decoration: none;
  font-weight: 500;
  transition: color 0.3s ease;
  display: flex;
  align-items: center;
  padding: 5px 0;
}

.nav-link::before {
  content: "▹";
  color: #64ffda;
  margin-right: 10px;
  font-size: 0.8rem;
  transition: transform 0.2s ease;
}

.nav-link:hover,
.router-link-exact-active,
.active-section {
  color: #64ffda;
}

.nav-link:hover::before,
.router-link-exact-active::before,
.active-section::before {
  transform: translateX(3px);
}

/* Footer social */
.sidebar-footer {
  display: flex;
  justify-content: flex-end;
  align-items: center;
  gap: 20px;
}

.sidebar-footer a {
  color: #8892b0;
  font-size: 1.5rem;
  transition: all 0.3s ease;
}

.sidebar-footer a:hover {
  color: #64ffda;
  transform: translateY(-3px);
}

@media (max-width: 768px) {
  .sidebar {
    width: 100%;
    height: auto;
    padding: 20px;
    position: relative;
    border-right: none;
    border-bottom: 1px solid #233554;
  }

  .sidebar-content {
    flex-direction: column;
  }

  .sidebar-top {
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
  }
  
  /* Cambios para nav y footer en mobile/tablet */
  .nav-footer-container {
    flex-direction: column;
    align-items: center;
    gap: 20px;
    margin: 20px 0;
  }

  .sidebar-nav {
    width: 100%;
    margin: 0;
  }

  .sidebar-nav ul {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 15px;
  }

  .sidebar-nav li {
    margin-bottom: 0;
  }
  
  .sidebar-footer {
    width: 100%;
    justify-content: center;
    padding-top: 15px;
    border-top: 1px solid #233554;
  }

  .bio {
    text-align: center;
  }
}
</style>
  