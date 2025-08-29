<template>
  <div class="intro">
    <div class="intro_text">

      <div class="intro_main">
        Bienvenue sur mon portfolio
      </div>
      <div class="intro_sub">
        Mathis BEAL, développeur logiciel passionné
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">

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


.intro {
  width: 100%;
  height: 30rem;
  background-image: url('public/intro_back.png');
  background-position: center center;
  background-repeat: no-repeat;
  background-size: cover;
  display: flex;
  align-items: center;
  justify-content: center;
}

.intro_text {
  height: fit-content;
  padding: 0.5rem;
  padding-right: 5.5rem;
  font-weight: bold;
  margin: auto;
  color: rgb(224, 224, 224);
  background: radial-gradient(circle, rgba(83, 83, 83, 0.8) 40%, rgb(73, 73, 73) 100%);
  border-radius: 1rem;
  /* optional, for rounded corners */
  border: solid 0.6rem white;
  box-shadow: 0.4rem 0.4rem 0.4rem rgba(255, 255, 255, 0.5);
}

.intro_main {
  font-size: 2.2rem;
}

.intro_sub {
  font-size: 1.7rem;
  position: relative;
  left: 5rem;
}
</style>
