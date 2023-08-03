<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <div class="container">
    <header>
      <nav class="navigation-panel">
        <div class="navigation-header">
          <img src="./assets/logo.svg" width="200"/>
          <h1>X</h1>
        </div>
        <div class="navigation-buttons">
          <RouterLink to="/">Home</RouterLink>
          <RouterLink to="/about">About</RouterLink>
        </div>
      </nav>
    </header>
    <RouterView />
  </div>
</template>

<style scoped>

header {
  position: fixed;
  z-index: 200;
}
.navigation-panel {
  background-color: var(--color-background-soft);
  height: 100vh;
  width: 400px;
}

.navigation-buttons {
  display: grid;
  gap: 20px;
}

.navigation-header {
  display: flex;
  justify-content: space-between;
}
</style>
