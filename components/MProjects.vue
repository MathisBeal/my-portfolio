<template>
  <div class="main_div">
    <div class="make">
      <h2>Mes projets ? <span class="make_highlight">$make</span></h2>
    </div>
    <div class="carousel">
      <button class="carousel-btn" @click="prev">&#8592;</button>
      <NuxtLink :to="projects[current]?.link" class="carousel-item">
        <img :src="projects[current]?.img" alt="Image projet" class="carousel-img" />
        <div class="carousel-text">{{ projects[current]?.text }}</div>
      </NuxtLink>
      <button class="carousel-btn" @click="next">&#8594;</button>
    </div>
  </div>
</template>

<script lang="ts" setup>
import { ref } from 'vue'

const projects = [
  {
    img: '/Nutriplan/logo_nutriplan.png',
    text: 'Nutriplan : Application web de suivi nutritionnel',
    link: '/nutriplan'
  },
  {
    img: '/Power4/Puissance4.png',
    text: 'IA : Intelligence artificielle sur le jeu du Puissance 4',
    link: '#'
  },
  {
    img: '/Tractopel/Tractopel.jpeg',
    text: 'Contrôle d\'un véhicule articulé à l\'aide d\'une application Android',
    link: '#'
  },
  {
    img: '/Museum/Museum.png',
    text: 'Musée 3D : Visite virtuelle d\'un musée',
    link: '#'
  }
]

const current = ref(0)
const prev = () => { if (current.value > 0) current.value--; else current.value = projects.length - 1; }
const next = () => { if (current.value < projects.length - 1) current.value++; else current.value = 0 }
</script>

<style scoped>
.make {
  font-size: 1.8rem;
  width: fit-content;
  margin: auto;
  border-top: 0.2rem solid #3fa36b;
  border-bottom: 0.2rem solid #3fa36b;
  padding: 0.5rem 0;
}

.make_highlight {
  font-family: Consolas, monospace;
  color: #3fa36b;
  font-weight: bold;
  font-size: 1.1em;
}

.carousel {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 2rem;
  margin: 2rem auto;
}
.carousel-item {
  display: flex;
  flex-direction: column;
  align-items: center;
  background: #f8f8f8;
  border-radius: 1rem;
  box-shadow: 0 2px 8px rgba(0,0,0,0.08);
  padding: 1.5rem;
  min-width: 18rem;
  max-width: 22rem;
}
.carousel-img {
  width: 100%;
  max-width: 50vw;
  max-height: 50vh;
  object-fit: contain;
  margin-bottom: 1rem;
  border-radius: 0.5rem;
  background: #eaeaea;
}
.carousel-text {
  font-size: 1.25rem;
  color: #2c3e50;
  text-align: center;
  transition: color 0.2s, font-weight 0.2s;
  text-decoration: underline #2c3e50;
}
.carousel-item:hover .carousel-text {
  color: #3fa36b;
  text-decoration: underline #3fa36b;
  font-weight: bold;
}
.carousel-btn {
  background: #3fa36b;
  color: white;
  border: none;
  border-radius: 0.5rem;
  padding: 0.7rem 1.2rem;
  font-size: 1.5rem;
  cursor: pointer;
  transition: background 0.2s;
}
.carousel-btn:disabled {
  background: #b2b2b2;
  cursor: not-allowed;
}
.carousel-btn:not(:disabled):hover {
  background: #31905a;
}
.main_div {
  max-width: 90vw;
  margin: 3rem auto;
}
</style>