<template>
  <div>
  </div>
  <footer :class="['footer', sticky ? 'footer-sticky' : '']">
    <div class="footer-main">
      &copy; 2025 Mathis BEAL — Tous droits réservés
    </div>
    <div class="footer-links">
      <NuxtLink to="/mentions-legales" class="footer-link">Mentions légales</NuxtLink>
      <span class="footer-sep">|</span>
      <NuxtLink to="/site-plan" class="footer-link">Plan du site</NuxtLink>
      <span class="footer-sep">|</span>
      <a href="https://github.com/mathisbeal" class="footer-link" target="_blank" rel="noopener">
        <span class="footer-icon">🐙</span> GitHub
      </a>
      <span class="footer-sep">|</span>
      <a href="https://www.linkedin.com/in/mathis-beal/" class="footer-link" target="_blank" rel="noopener">
        <span class="footer-icon">in</span> LinkedIn
      </a>
    </div>
  </footer>
</template>

<script lang="ts" setup>
defineProps<{ sticky?: boolean }>()
</script>

<style scoped>
.footer {
  width: 100%;
  background: #2c3e50;
  color: #fff;
  padding: 1.2rem 0 0.7rem 0;
  text-align: center;
  font-size: 1rem;
  border-top: 2px solid #3fa36b;
  margin-top: auto;
}
.footer-sticky {
  position: fixed;
  left: 0;
  bottom: 0;
  z-index: 100;
  margin-top: 0;
}
.footer-main {
  margin-bottom: 0.5rem;
}
.footer-links {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 0.7rem;
  flex-wrap: wrap;
}
.footer-link {
  color: #3fa36b;
  text-decoration: none;
  font-weight: bold;
  transition: color 0.2s;
  display: flex;
  align-items: center;
  gap: 0.3rem;
}
.footer-link:hover {
  color: #31905a;
  text-decoration: underline;
}
.footer-sep {
  color: #fff;
  font-weight: normal;
}

/* Ajout d'icônes simples pour GitHub et LinkedIn */
.footer-icon {
  font-size: 1.2em;
}
</style>