<template>
  <div class="app-layout">
    <Sidebar />
    <main class="main-content">
      <RouterView />
    </main>
    <!-- <div v-if="showGlow" :style="glowStyle" class="cursor-glow"></div> -->
  </div>
</template>

<script setup>
import { ref, computed, onMounted, onUnmounted } from 'vue'
import Sidebar from './components/Sidebar.vue'


</script>

<style scoped>
</style>

<style>
/* Estilos globales (fuera del scope del componente) */
.app-layout {
  display: flex;
  justify-content: center;
  min-height: 100vh;
  background: radial-gradient(ellipse at 50% 0%, #233554 0%, #0a192f 100%);
}

.main-content {
  flex: 1;
  overflow-y: auto;
  height: 100vh;
  padding: 40px 32px;
  color: #ccd6f6;
  margin-left: 250px; /* Ajusta según sea necesario, el mismo valor que el ancho del sidebar */
}
</style>
