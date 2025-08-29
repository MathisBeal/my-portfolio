<template>
  <header class="header">
    <div class="header-left">
      Mathis BÉAL
    </div>
    <nav class="header-right">
      <NuxtLink to="/">Accueil</NuxtLink>
      <NuxtLink to="/#about">À propos</NuxtLink>
      <NuxtLink to="/#parcours">Parcours</NuxtLink>
      <NuxtLink to="/#projects">Projets</NuxtLink>
      <a href="/#cv">Mon CV</a>
    </nav>
  </header>
</template>

<script setup>
// No script needed for static header
</script>

<style scoped>

.header {
  position: sticky;
  top: 0;
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  background: var(--mgreen);
  box-shadow: 0 2px 8px rgba(0,0,0,0.05);
  padding: 1rem 1rem;      /* Adds space on left and right */
  margin: 0 auto;       /* Centers header if max-width is set */
  box-sizing: border-box;
  z-index: 100;
  font-size: 1.25rem;
}
.header-left {
  font-weight: bold;
  font-size: larger;
}
.header-right {
  display: flex;
  gap: 1.5rem;
  padding-right: 2rem;
}
.header-right a {
  text-decoration: none;
  color: #333;
  font-weight: 500;
  transition: color 0.2s;
}
.header-right a:hover {
  color: #007bff;
}
</style>