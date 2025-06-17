<template>
  <div id="app">
    <nav class="navbar">
      <div class="nav-container">
        <h1 class="logo">Florent Lin</h1>
        <ul class="nav-links">
          <li>
            <a
              href="#"
              @click="currentView = 'home'"
              :class="{ active: currentView === 'home' }"
              >Accueil</a
            >
          </li>
          <li>
            <a
              href="#"
              @click="currentView = 'cv'"
              :class="{ active: currentView === 'cv' }"
              >CV</a
            >
          </li>
          <!-- Vous pouvez ajouter d'autres liens ici -->
        </ul>
      </div>
    </nav>

    <main class="main-content">
      <!-- Page d'accueil simple -->
      <div v-if="currentView === 'home'" class="home-page">
        <div class="hero">
          <h1>Bienvenue sur mon site personnel</h1>
          <p>Ingénieur en Data Sciences - ENSAE Paris</p>
          <button @click="currentView = 'cv'" class="cta-button">
            Voir mon CV
          </button>
        </div>
      </div>

      <!-- Page CV -->
      <CVPage v-else-if="currentView === 'cv'" />
    </main>
  </div>
</template>

<script setup lang="ts">
import { ref } from "vue";
import CVPage from "./views/CVPage.vue";

const currentView = ref<"home" | "cv">("home");
</script>

<style>
/* Reset et styles globaux */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen,
    Ubuntu, Cantarell, sans-serif;
  color: #333;
  background-color: #f5f5f5;
}

#app {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
}

/* Navigation */
.navbar {
  background-color: #1a1a1a;
  color: white;
  padding: 1rem 0;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.nav-container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 20px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo {
  font-size: 1.5rem;
  font-weight: bold;
}

.nav-links {
  display: flex;
  list-style: none;
  gap: 2rem;
}

.nav-links a {
  color: white;
  text-decoration: none;
  transition: color 0.3s ease;
  padding: 0.5rem 1rem;
  border-radius: 4px;
}

.nav-links a:hover {
  color: #3b82f6;
}

.nav-links a.active {
  background-color: #3b82f6;
  color: white;
}

/* Contenu principal */
.main-content {
  flex: 1;
}

/* Page d'accueil */
.home-page {
  display: flex;
  align-items: center;
  justify-content: center;
  min-height: calc(100vh - 70px);
  padding: 2rem;
}

.hero {
  text-align: center;
  max-width: 600px;
}

.hero h1 {
  font-size: 3rem;
  margin-bottom: 1rem;
  color: #1a1a1a;
}

.hero p {
  font-size: 1.25rem;
  color: #666;
  margin-bottom: 2rem;
}

.cta-button {
  background-color: #3b82f6;
  color: white;
  border: none;
  padding: 12px 30px;
  font-size: 1.1rem;
  border-radius: 6px;
  cursor: pointer;
  transition: all 0.3s ease;
}

.cta-button:hover {
  background-color: #2563eb;
  transform: translateY(-2px);
  box-shadow: 0 4px 12px rgba(59, 130, 246, 0.4);
}

/* Responsive */
@media (max-width: 768px) {
  .nav-container {
    flex-direction: column;
    gap: 1rem;
  }

  .hero h1 {
    font-size: 2rem;
  }

  .hero p {
    font-size: 1rem;
  }
}
</style>
