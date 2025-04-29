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

<style>
.app-layout {
  display: flex;
  min-height: 100vh;
  max-width: 1600px;
  margin: 0 auto;
  /* background: radial-gradient(ellipse at 50% 0%, #233554 0%, #0a192f 100%); */
}

.main-content {
  flex: 1;
  padding: 0 50px;
  color: #ccd6f6;
}

@media (max-width: 768px) {
  .app-layout {
    flex-direction: column;
  }
  
  .main-content {
    padding: 0 20px;
  }
}
</style>
