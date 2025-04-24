<template>
  <div class="app-layout">
    <Sidebar />
    <main class="main-content">
      <RouterView />
    </main>
    <div v-if="showGlow" :style="glowStyle" class="cursor-glow"></div>
  </div>
</template>

<script setup>
import { ref, computed, onMounted, onUnmounted } from 'vue'
import Sidebar from './components/Sidebar.vue'

const glowX = ref(0)
const glowY = ref(0)
const showGlow = ref(false)

const glowStyle = computed(() => ({
  left: `${glowX.value - 250}px`,
  top: `${glowY.value - 250}px`,
}))

function handleMouseMove(e) {
  glowX.value = e.clientX
  glowY.value = e.clientY
  showGlow.value = true
}
function handleMouseLeave() {
  showGlow.value = false
}

onMounted(() => {
  window.addEventListener('mousemove', handleMouseMove)
  window.addEventListener('mouseleave', handleMouseLeave)
})
onUnmounted(() => {
  window.removeEventListener('mousemove', handleMouseMove)
  window.removeEventListener('mouseleave', handleMouseLeave)
})
</script>

<style scoped>
/* Estilos para el glow */
.cursor-glow {
  position: fixed;
  width: 400px;
  height: 400px;
  pointer-events: none;
  border-radius: 50%;
  background: radial-gradient(circle, rgba(255, 255, 255, 0.25) 0%, rgba(255, 255, 255, 0.1) 50%, transparent 80%);
  z-index: 9999;
  transition: left 0.08s, top 0.08s;
  mix-blend-mode: lighten;
}
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
