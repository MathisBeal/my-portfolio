<template>
  <div class="main_div">
    <MHeader />
    <div class="site-plan">
      <div class="title">
        <h1>Plan du site</h1>
      </div>
      <ul class="site-plan-list">
        <li><a href="/">Accueil</a></li>
        <li>
          Projets :
          <ul class="site-plan-sublist">
            <li><a href="/nutriplan">Nutriplan</a></li>
            <li><a href="/power-ai">Power AI</a></li>
            <li><a href="/tractopel">Tractopel</a></li>
            <li><a href="/museum">Musée 3D</a></li>
          </ul>
        </li>
        <li><a href="/cv">Mon CV</a></li>
        <li><a href="/mentions-legales">Mentions légales</a></li>
        <li><a href="/site-plan">Plan du site</a></li>
      </ul>
    </div>
    <MFooter sticky/>
  </div>
</template>

<script lang="ts" setup>

</script>

<style scoped>
.main_div {
  display: flex;
  flex-direction: column;
  align-items: center;
  /* background: #f8f8f8; */
}
.site-plan {
  width: 50vw;
  background: #f8f8f8;
  max-width: 32rem;
  margin: 3rem auto;
  margin-top: 0;
  box-shadow: 0 2px 12px rgba(63,163,107,0.10);
  padding: 2rem 2.5rem;
  color: #2c3e50;
}
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
.site-plan-list {
  list-style: none;
  padding: 0;
}
.site-plan-list li {
  margin: 1rem 0;
}
.site-plan-list a {
  color: #3fa36b;
  font-weight: bold;
  text-decoration: none;
  font-size: 1.15rem;
  transition: color 0.2s;
}
.site-plan-list a:hover {
  color: #31905a;
  text-decoration: underline;
}
.site-plan-sublist {
  list-style: none;
  padding-left: 2rem;
  margin: 0.5rem 0;
}
.site-plan-sublist li {
  margin: 0.5rem 0;
}
</style>