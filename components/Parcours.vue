<template>
  <div class="main_div">
        <div class="ls">
      <h2>Mon parcours <span class="ls_highlight">$ls</span></h2>
    </div>
    <div class="event right future">
      <div class="year">2025 - 2027</div>
      <div class="content">
        <div>
          <span class="title">Master en cybersécurité</span>
          <ul>
            <li>BAC +5</li>
            <li>En alternance</li>
          </ul>
        </div>
        <img src="/logo_cfai.png" alt="Logo CFAI" class="content-img">
      </div>
    </div>
    <div class="event left">
      <div class="year">2024 - 2025</div>
      <div class="content">
        <div>
          <span class="title">Développeur logiciel embarqué chez SAM Outillage (Alternance)</span>
          <ul>
            <li>Développement de logiciel embarqué</li>
            <li>Utilisation de Rust, Java</li>
            <li>Utilisation de périphériques</li>
          </ul>
        </div>
        <img src="/logo_sam.png" alt="Logo SAM Outillage" class="content-img">
      </div>
    </div>
    <div class="event right">
      <div class="year">2024</div>
      <div class="content">
        <div>
          <span class="title">Développeur web chez Isitecc (Stage)</span>
          <ul>
            <li>Développement sur une application web</li>
            <li>Utilisation de MSSQL, React, .NET</li>
          </ul>
        </div>
        <img src="/logo_isitecc.png" alt="Logo Isitecc" class="content-img">
      </div>
    </div>
        <div class="event left">
      <div class="year">2022 - 2025</div>
      <div class="content">
        <div>
          <span class="title">BUT Informatique</span>
          <p>
            De nombreux projets réalisés au cours de cette formation, sur du logiciel, 
            web ou jeu vidéo, pour la plupart en équipe
          </p>
        </div>
        <img src="/logo_iut.png" alt="Logo IUT" class="content-img">
      </div>
    </div>

  </div>
</template>

<script lang="ts" setup>

</script>

<style scoped>
.main_div {
  padding: 3rem;
  height: fit-content;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  font-size: 1.3rem;
  color: white;
  background-color: #2e5f91;
  font-weight: normal;
  gap: 2rem;
}

.ls {
  font-size: 1.8rem;
  width: fit-content;
  margin: auto;
  border-top: 0.2rem solid #3fa36b;
  border-bottom: 0.2rem solid #3fa36b;
  padding: 0.5rem 0;
}

.ls_highlight {
  font-family: Consolas, monospace;
  color: #3fa36b;
  font-weight: bold;
  font-size: 1.1em;
}


.year {
  text-align: center;
  font-size: larger;
  font-weight: bold;
}

.event {
  padding: 1rem;
  max-width: 30vw;
  border: 0.4rem solid var(--mgreen);
  display: flex;
  flex-direction: column;
  align-items: center;
  background: whitesmoke;
  color: black;
}

.future {
  background: rgba(245, 245, 245, 0.85);
  border: 0.4rem dashed var(--mgreen);
}

.content {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.content-img {
  margin: 1rem auto 0 auto;
  display: block;
  max-width: 20rem;
  max-height: 7rem;
  object-fit: contain;
}

.title {
  font-size: 1.5rem;
}

.left {
  position: relative;
  left: -20vw;
}

.right {
  position: relative;
  right: -20vw;
}
</style>