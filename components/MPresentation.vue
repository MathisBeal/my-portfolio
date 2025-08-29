<template>
  <div class="main_div">
    <div class="whoami">
      <h2>Qui suis-je ? <span class="whoami_highlight">$whoami</span></h2>
    </div>
    <div class="block">
      <div class="text">
        <p>
          Salut 👋 Moi c'est Mathis BÉAL, développeur junior passionné par le développement logiciel.
          Actuellement agé de {{ yearsSince2004 }} ans, je suis en dernière année de BUT Informatique (BAC +3)
          <br /><br />
          J'envisage ensuite de continuer en Master Informatique spécialisé en Cybersécurité, m'amenant ainsi à un
          diplôme de niveau Bac +5.
        </p>
      </div>
      <img src="/public/pp.jpeg" alt="Photo de Mathis BÉAL" class="pp" />
    </div>
  </div>
</template>

<script lang="ts" setup>
const yearsSince2004 = (() => {
  const startDate = new Date(2004, 6, 19) // Months are 0-indexed: 6 = July
  const now = new Date()
  let years = now.getFullYear() - startDate.getFullYear()
  if (
    now.getMonth() < startDate.getMonth() ||
    (now.getMonth() === startDate.getMonth() && now.getDate() < startDate.getDate())
  ) {
    years--
  }
  return years
})()
</script>

<style scoped>
.whoami {
  font-size: 1.8rem;
  width: fit-content;
  margin: auto;
  border-top: 0.2rem solid #3fa36b;
  border-bottom: 0.2rem solid #3fa36b;
  padding: 0.5rem 0;
}

.whoami_highlight {
  font-family: Consolas, monospace;
  color: #3fa36b;
  font-weight: bold;
  font-size: 1.1em;
}

.pp {
  max-width: 40%;
  max-height: 25vw;
  object-fit: contain;
  border: 0.2rem solid #3fa36b;
  box-shadow: 1rem 1rem 0.2rem rgba(63, 163, 106, 0.65);
}

.main_div {
  padding: 3rem;
  margin-bottom: 5rem;
}

.block {
  margin: auto;
  max-width: 65vw;
  display: flex;
  flex-direction: row;
  gap: 2rem;
  align-items: center;
  justify-content: space-between;
  margin-top: 2rem;
}

.text {
  max-width: 60%;
  font-size: 1.2rem;
  line-height: 1.6;
}
</style>