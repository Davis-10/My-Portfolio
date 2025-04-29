<template>
  <section id="projects">
    <h2 class="section-heading">Proyectos</h2>

    <div class="projects-container">
      <div class="project-card">
        <div class="project-content">
          <div class="project-header">
            <h3 class="project-title">FantasyRace</h3>
          </div>
          <div class="project-description">
            <p>
              Este proyecto es un juego basado en los resultados de las competiciones
              de Fórmula 1 o carreras de Grand Prix celebradas desde el año 2000 hasta
              la actualidad. El juego consta de los siguientes pasos: 1. Seleccionar
              un año. 2. Elegir una de las carreras celebradas ese año. 3. Seleccionar
              uno de los equipos (escuderías) que participaron en la carrera. 4.
              Finalmente, elegir uno de los pilotos del equipo seleccionado que
              compitió en la carrera.
            </p>
          </div>
          <ul class="tech-list">
            <li>
              <font-awesome-icon :icon="['fab', 'vuejs']" class="tech-logo" />
              Vue.js
            </li>
            <li>
              <font-awesome-icon :icon="['fab', 'js']" class="tech-logo" />
              JavaScript
            </li>
            <li>
              <font-awesome-icon :icon="['fab', 'css3']" class="tech-logo" />
              CSS
            </li>
          </ul>
          <div class="project-links">
            <a
              href="https://jolly-strudel-a6e71c.netlify.app/"
              target="_blank"
              rel="noopener noreferrer"
              class="project-link"
            >
              <font-awesome-icon :icon="['fas', 'external-link-alt']" class="link-icon" />
              Ver proyecto
            </a>
          </div>
        </div>
        <div class="project-image">
          <div class="image-container">
            <img src="@/assets/preview_FantasyRace.png" alt="Previsualización de FantasyRace" />
          </div>
        </div>
      </div>

      <div class="project-card">
        <div class="project-content">
          <div class="project-header">
            <h3 class="project-title">Illustre - Ecommerce Bisuteria</h3>
          </div>
          <div class="project-description">
            <p>
              ILLUSTRE es un proyecto de tienda online de bisutería desarrollado en
              equipo. La página ofrece una experiencia completa con tres secciones
              principales: Tienda: Explora nuestro catálogo de bisutería. Nosotros:
              Conoce nuestra historia y equipo. Contacto: Contáctanos para cualquier
              consulta. Además, incluye secciones secundarias para una gestión
              integral: Producto: Detalle de cada artículo. Usuario: Gestión de
              perfiles de cliente. Administrador: Panel de control para la
              administración de la tienda.
            </p>
          </div>
          <ul class="tech-list">
            <li>
              <font-awesome-icon :icon="['fab', 'js']" class="tech-logo" />
              JavaScript
            </li>
            <li>
              <font-awesome-icon :icon="['fab', 'html5']" class="tech-logo" />
              HTML5
            </li>
            <li>
              <font-awesome-icon :icon="['fab', 'css3']" class="tech-logo" />
              CSS3
            </li>
          </ul>
          <div class="project-links">
            <a
              href="https://delicate-seahorse-c9fef8.netlify.app/"
              target="_blank"
              rel="noopener noreferrer"
              class="project-link"
            >
              <font-awesome-icon :icon="['fas', 'external-link-alt']" class="link-icon" />
              Ver proyecto
            </a>
          </div>
        </div>
        <div class="project-image">
          <div class="image-container">
            <img src="@/assets/preview_Illustre.png" alt="Previsualización de Illustre" />
          </div>
        </div>
      </div>

      <div class="project-card">
        <div class="project-content">
          <div class="project-header">
            <h3 class="project-title">Blog de Café</h3>
          </div>
          <div class="project-description">
            <p>
              Este proyecto es un blog dedicado a los amantes del café, donde se
              publican artículos sobre diferentes tipos de granos, métodos de
              preparación y cultura cafetera. Además, cuenta con cursos especializados
              para que los usuarios puedan ampliar sus conocimientos y habilidades en
              el mundo del café. La página incluye también una sección de contacto
              para facilitar la comunicación con los visitantes interesados.
            </p>
          </div>
          <ul class="tech-list">
            <li>
              <font-awesome-icon :icon="['fab', 'html5']" class="tech-logo" />
              HTML5
            </li>
            <li>
              <font-awesome-icon :icon="['fab', 'css3']" class="tech-logo" />
              CSS3
            </li>
          </ul>
          <div class="project-links">
            <a 
              href="https://gleaming-bavarois-256825.netlify.app/" 
              target="_blank" 
              rel="noopener noreferrer"
              class="project-link"
            >
              <font-awesome-icon :icon="['fas', 'external-link-alt']" class="link-icon" />
              Ver proyecto
            </a>
          </div>
        </div>
        <div class="project-image">
          <div class="image-container">
            <img src="@/assets/preview_BlogCafe.png" alt="Previsualización de Blog de Café" />
          </div>
        </div>
      </div>

      <div class="project-card">
        <div class="project-content">
          <div class="project-header">
            <h3 class="project-title">Asociación Pádel Amorebieta</h3>
          </div>
          <div class="project-description">
            <p>
              Landing Page de Jugadores de Padel. Participé en este proyecto ya
              avanzado, contribuyendo con el desarrollo de una landing page. Esta
              sección muestra información clave de los jugadores afiliados a la
              asociación o club deportivo de pádel, presentando sus imágenes y datos
              principales de manera atractiva y organizada.
            </p>
          </div>
          <ul class="tech-list">
            <li>
              <font-awesome-icon :icon="['fab', 'html5']" class="tech-logo" />
              HTML5
            </li>
            <li>
              <font-awesome-icon :icon="['fab', 'css3']" class="tech-logo" />
              CSS3
            </li>
          </ul>
          <div class="project-links">
            <a 
              href="https://sprightly-figolla-303c3a.netlify.app/jugadores" 
              target="_blank" 
              rel="noopener noreferrer"
              class="project-link"
            >
              <font-awesome-icon :icon="['fas', 'external-link-alt']" class="link-icon" />
              Ver proyecto
            </a>
          </div>
        </div>
        <div class="project-image">
          <div class="image-container">
            <img src="@/assets/preview_JUgadoresPadel.png" alt="Previsualización de Asociación Pádel Amorebieta" />
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
#projects {
  max-width: 1000px;
  margin: 0 auto;
  padding: 100px 0;
}

.section-heading {
  font-size: 2.5rem;
  margin-bottom: 50px;
  position: relative;
  display: inline-block;
}

.section-heading::after {
  content: '';
  position: absolute;
  bottom: -10px;
  left: 0;
  width: 70%;
  height: 4px;
  background-color: #64ffda;
}

.projects-container {
  display: flex;
  flex-direction: column;
  gap: 100px;
}

.project-card {
  display: grid;
  grid-template-columns: repeat(12, 1fr);
  position: relative;
}

.project-content {
  grid-column: 1 / 8;
  grid-row: 1 / -1;
  position: relative;
  z-index: 2;
}

.project-image {
  grid-column: 6 / -1;
  grid-row: 1 / -1;
  position: relative;
}

.project-card:nth-child(even) .project-content {
  grid-column: 6 / -1;
  text-align: right;
}

.project-card:nth-child(even) .project-image {
  grid-column: 1 / 8;
}

.project-card:nth-child(even) .tech-list {
  justify-content: flex-end;
}

.project-title {
  font-size: 1.8rem;
  margin-bottom: 20px;
  color: #e6f1ff;
}

.project-description {
  background-color: #112240;
  padding: 25px;
  border-radius: 4px;
  box-shadow: 0 10px 30px -15px rgba(2, 12, 27, 0.7);
  transition: transform 0.3s ease;
  margin-bottom: 20px;
}

.project-card:hover .project-description {
  transform: translateY(-7px);
}

.project-description p {
  margin: 0;
  line-height: 1.7;
  color: #a8b2d1;
  text-align: justify;
}

.tech-list {
  display: flex;
  flex-wrap: wrap;
  margin: 20px 0;
  padding: 0;
  list-style: none;
  gap: 10px;
}

.tech-list li {
  background-color: #172a45;
  padding: 7px 12px;
  border-radius: 3px;
  font-size: 0.9rem;
  font-family: monospace;
  display: flex;
  align-items: center;
  transition: background-color 0.3s ease;
}

.tech-list li:hover {
  background-color: #233554;
}

.tech-logo {
  margin-right: 8px;
  font-size: 1rem;
}

.project-links {
  display: flex;
  gap: 15px;
  margin-top: 15px;
}

.project-card:nth-child(even) .project-links {
  justify-content: flex-end;
}

.project-link {
  color: #64ffda;
  text-decoration: none;
  font-size: 1rem;
  display: flex;
  align-items: center;
  transition: all 0.3s ease;
}

.project-link:hover {
  transform: translateY(-3px);
  color: #64ffda;
}

.link-icon {
  margin-right: 8px;
}

.image-container {
  height: 100%;
  width: 100%;
  border-radius: 4px;
  overflow: hidden;
  position: relative;
  background-color: #64ffda;
  transition: all 0.3s ease;
}

.image-container::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: #0a192f;
  opacity: 0.7;
  z-index: 1;
  transition: opacity 0.3s ease;
}

.project-card:hover .image-container::before {
  opacity: 0.2;
}

.image-container img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  object-position: center;
  position: relative;
  z-index: 0;
  filter: grayscale(100%);
  transition: all 0.3s ease;
}

.project-card:hover .image-container img {
  filter: grayscale(0);
}

@media (max-width: 768px) {
  .project-card {
    grid-template-columns: 1fr;
  }
  
  .project-content,
  .project-card:nth-child(even) .project-content {
    grid-column: 1 / -1;
    padding: 20px;
    text-align: left;
  }
  
  .project-image,
  .project-card:nth-child(even) .project-image {
    grid-column: 1 / -1;
    height: 300px;
  }
  
  .tech-list,
  .project-card:nth-child(even) .tech-list,
  .project-links,
  .project-card:nth-child(even) .project-links {
    justify-content: flex-start;
  }
  
  .project-description {
    padding: 20px;
  }
}
</style>
