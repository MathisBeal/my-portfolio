<template>
  <div>
    <m-header />
    <div class="main_div">
      <div class="title">
        <h1 class="ls">Nutriplan</h1>
      </div>
      <div class="short_desc">
        Application web de suivi nutritionnel
      </div>
      <div class="part">
        <div class="sub-part ">
          <div class="part_title">
            <h2>Contexte</h2>
          </div>
          <div class="part_text">
            Dans le cadre d'un projet universitaire, nous avons eu environ 1 mois, avec une équipe de 4 personnes, pour
            réaliser notre application.<br />
            L'objectif était d'apprendre à utiliser de nouvelles technologies et d'appliquer les connaissances acquises
            durant la formation.
            <br /><br /><br />
            L'utilisateur crée son profil en précisant ses préférences, allergies ou régime, puis explore des recettes
            et aliments détaillés qu'il peut ajouter en favoris. L'application lui suggère des plats adaptés aux
            ingrédients disponibles et à ses besoins, tout en offrant un suivi de l'alimentation et de l'hydratation
            avec des bilans et graphiques clairs. Grâce à un système de recherche et de filtres avancés, il trouve
            facilement ce qu'il cherche, le tout dans une expérience simple et personnalisée pour favoriser une
            alimentation plus saine.
          </div>
        </div>
        <img src="/public/Nutriplan/logo_nutriplan.png" alt="Logo Nutriplan">
      </div>
      <div class="part">
        <img src="/public/Nutriplan/Nutriplan.png" alt="Logo Nutriplan">
        <div class="sub-part ">
          <div class="part_title">
            <h2>Organisation</h2>
          </div>
          <div class="part_text">
            Pour mener ce projet à bien, on a mis en place des méthodes de travail afin de se répartir les tâches<br />
            Chaque membre de l'équipe a pris en charge une partie du projet en fonction de ses compétences et de ses
            intérêts. <br />
            <br />
            On a commencé le travail par choisir les technologies que l'on allais utiliser, mais aussi essayer de
            trouver des sources de données à utiliser. <br>
            Je me suis occupé de gérer l'affichage des recettes, des aliments, et des différents détails les concernant.
            <br>
            J'ai également travailler sur l'API qui nous permettait de communiquer avec notre base de donnée, en
            particulier sur la partie à propos des recettes et des aliments, quels informations récupérer dans la base
            lorsqu'on veut afficher une recette.
            <br><br>
            J'ai aussi participé aux autres tâches, comme la création de la base de donnée, gérer le déploiement de la
            base de donnée et du site, et aider à résoudre les problèmes qu'on pouvait rencontrer.
          </div>
        </div>
      </div>
      <div class="part">
        <div class="sub-part ">
          <div class="part_title">
            <h2>Conclusion</h2>
          </div>
          <div class="part_text">
            Lors de ce projet, nous avons été confrontés à un manque de temps qui ne nous a pas permis d'atteindre
            l'ensemble des objectifs fixés. Cependant, cette expérience nous a permis de consolider nos compétences, de
            mieux comprendre la gestion des priorités dans un projet.
            <br /><br />
            Nous avons tout de même pu confirmer l'efficacité des technologies choisies, qui ici étaient plus orientées
            dans du développement et maintien d'application à long terme et non pas de développer rapidement sans
            prendre en compte les complexités à venir.
            <br><br>
            J'ai pu acquérir et renforcer mes compétences techniques sur l'ensemble des technologies suivantes mais
            aussi mes softs skills grâce au travail en équipe et méthodes de travail fixées.
          </div>
        </div>
      </div>
      <div class="tech-title">
        <h2>Les technologies utilisées</h2>
      </div>
      <div class="image-rows">
        <div class="image-row">
          <div class="image-item">
            <img src="/Nutriplan/techs/github.png" alt="GitHub" />
            <div class="image-text">GitHub</div>
          </div>
          <div class="image-item">
            <img src="/Nutriplan/techs/vue.png" alt="Vue.js" />
            <div class="image-text">Vue.js</div>
          </div>
          <div class="image-item">
            <img src="/Nutriplan/techs/nuxt.png" alt="Nuxt.js" />
            <div class="image-text">Nuxt.js</div>
          </div>
        </div>
        <div class="image-row">
          <div class="image-item">
            <img src="/Nutriplan/techs/ts.png" alt="TypeScript" />
            <div class="image-text">TypeScript</div>
          </div>
          <div class="image-item">
            <img src="/Nutriplan/techs/mysql.png" alt="MySQL" />
            <div class="image-text">MySQL</div>
          </div>
          <div class="image-item">
            <img src="/Nutriplan/techs/docker.jpg" alt="Docker" />
            <div class="image-text">Docker</div>
          </div>
        </div>
      </div>
    </div>
    <m-footer />
  </div>
</template>

<script lang="ts" setup>

</script>

<style scoped>
.title {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: fit-content;
  text-align: center;
  color: #242424;
  margin-bottom: 2rem;
  border-bottom: 0.2rem solid #242424;
}

.short_desc {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: fit-content;
  text-align: center;
  color: #242424;
  margin-bottom: 2rem;
  font-size: 1.5rem;
}

.main_div {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 60vw;
  margin: auto;
  background: whitesmoke;
  padding: 0 2rem;
  gap: 3rem;
  /* background: #f8f8f8; */
}

.part {
  display: flex;
  flex-direction: row;
  align-items: center; /* changed from flex-start to center for vertical centering */
  gap: 2rem;
}

.sub-part {
  flex: 1;
  max-width: 60%;
  font-size: 1.1rem;
}

.part img {
  max-width: 40%;
  contain: content;
}

.context img,
.sub-part img {
  display: block;
  margin: auto 0;
}

.sub-part img {
  max-width: 12rem;
  max-height: 12rem;
  object-fit: contain;
  margin-left: 2rem;
  vertical-align: middle;
  border-radius: 1rem;
  box-shadow: 0 2px 8px rgba(63, 163, 107, 0.12);
  background: #f8f8f8;
  padding: 0.5rem;
}

.tech-title {
  text-align: center;
  margin-top: 3rem;
  margin-bottom: 0;
  color: #2c3e50;
  border-bottom: 0.2rem solid #2c3e50;
}

.tech-title h2 {
  font-size: 1.5rem;
  margin-bottom: 0;
  font-weight: bold;
}

.image-rows {
  margin: 0 auto 2rem auto;
  display: flex;
  flex-direction: column;
  gap: 2.5rem;
  align-items: center;
}

.image-row {
  display: flex;
  gap: 2.5rem;
  justify-content: center;
}

.image-item {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  background: #f8f8f8;
  border-radius: 1rem;
  box-shadow: 0 2px 8px rgba(63,163,107,0.10);
  padding: 1rem 1.2rem;
  min-width: 8rem;
}

.image-item img {
  display: block;
  margin: 0 auto;
  max-width: 6rem;
  max-height: 6rem;
  object-fit: contain;
  margin-bottom: 0.7rem;
  border-radius: 0.5rem;
  background: #eaeaea;
}

.image-text {
  font-size: 1rem;
  color: #2c3e50;
  text-align: center;
  margin-top: 0.2rem;
}
</style>