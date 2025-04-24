<template>
  <section id="projects">
    <h2>Some Things I’ve Built</h2>

    <div class="project-item">
      <h3>FantasyRace</h3>
      <p class="description">
        Este proyecto es un juego basado en los resultados de las competiciones
        de Fórmula 1 o carreras de Grand Prix celebradas desde el año 2000 hasta
        la actualidad. El juego consta de los siguientes pasos: 1. Seleccionar
        un año. 2. Elegir una de las carreras celebradas ese año. 3. Seleccionar
        uno de los equipos (escuderías) que participaron en la carrera. 4.
        Finalmente, elegir uno de los pilotos del equipo seleccionado que
        compitió en la carrera.
      </p>
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
      <a href="https://jolly-strudel-a6e71c.netlify.app/" target="_blank" rel="noopener noreferrer">
        Ver proyecto
      </a>
    </div>

    <div class="project-item">
      <h3>Illustre - Ecommerce Bisuteria</h3>
      <p class="description">
        ILLUSTRE es un proyecto de tienda online de bisutería desarrollado en
        equipo. La página ofrece una experiencia completa con tres secciones
        principales:Tienda: Explora nuestro catálogo de bisutería. Nosotros:
        Conoce nuestra historia y equipo. Contacto: Contáctanos para cualquier
        consulta.Además, incluye secciones secundarias para una gestión
        integral: Producto: Detalle de cada artículo.Usuario: Gestión de
        perfiles de cliente. Administrador: Panel de control para la
        administración de la tienda.
      </p>
      <ul class="tech-list">
        <li>
          <font-awesome-icon :icon="['fab', 'js']" class="tech-logo" />
          JavaScript
        </li>
        <li>
          <font-awseome-icon :icon="['fab', 'html5']" class="tech-logo" />
          HTML5
        </li>
        <li>
          <font-awesome-icon :icon="['fab', 'css3']" class="tech-logo" />
          CSS3
        </li>
      </ul>
      <a href="https://delicate-seahorse-c9fef8.netlify.app/" target="_blank" rel="noopener noreferrer">
        Ver proyecto
      </a>
    </div>

    <div class="project-item">
      <h3>Asociación Pádel Amorebieta</h3>
      <p class="description">
        Landing Page de Jugadores de Padel Participé en este proyecto ya
        avanzado, contribuyendo con el desarrollo de una landing page. Esta
        sección muestra información clave de los jugadores afiliados a la
        asociación o club deportivo de pádel, presentando sus imágenes y datos
        principales de manera atractiva y organizada.
      </p>
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
      <a href="[Link al proyecto]" target="_blank" rel="noopener noreferrer">
        Ver proyecto
      </a>
    </div>
  </section>
</template>

<style scoped>
section {
  max-width: 600px;
  margin: 0 auto;
  padding: 20px;
}

h2 {
  font-size: 2rem;
  margin-bottom: 20px;
}

.project-item {
  margin-bottom: 36px;
}

h3 {
  font-size: 1.5rem;
  margin-bottom: 5px;
}

.description {
  line-height: 1.6;
  margin-bottom: 10px;
  font-size: 1.2rem;
}

.tech-list {
  list-style: none;
  padding: 0;
  margin-bottom: 10px;
  display: flex;
  flex-wrap: wrap; /* Permite que los elementos se envuelvan a la siguiente línea */
}

.tech-list li {
  margin-right: 10px;
  margin-bottom: 5px;
  background-color: #233554;
  padding: 5px 10px;
  border-radius: 5px;
  display: flex;
  align-items: center;
}

.tech-logo {
  width: 20px; /* Ajusta el tamaño del logo */
  margin-right: 5px;
}

a {
  color: #64ffda;
  text-decoration: none;
}
</style>
