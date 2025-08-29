<template>
  <div class="main_div">
    <div class="man">
      <h2>Mon CV <span class="man_highlight">$man</span></h2>
    </div>
    <div class="div_cv">
      <img src="/public/CV.jpg" alt="Mon CV" class="cv_img" />
    </div>
    <div class="download_div">
      <a href="/CV.pdf" rel="noopener" target="_blank">Télécharger mon CV</a>
    </div>
  </div>
</template>

<script lang="ts" setup>

</script>

<style scoped>
.main_div {
  background: linear-gradient(120deg, #e8f5e9 70%, #c8e6c9 100%);
  box-shadow: 0 2px 16px rgba(63,163,107,0.10);
  padding: 2.5rem;
  margin: auto;
  margin-top: 3rem;
}

.man {
  font-size: 1.8rem;
  width: fit-content;
  margin: auto;
  border-top: 0.2rem solid #3fa36b;
  border-bottom: 0.2rem solid #3fa36b;
  padding: 0.5rem 0;
}

.man_highlight {
  font-family: Consolas, monospace;
  color: #3fa36b;
  font-weight: bold;
  font-size: 1.1em;
}

.div_cv {
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 1rem 0;
}

.cv_img {
  max-height: 70vh;
}

.download_div {
  text-align: center;
  margin: 1rem 0;
}

.download_div a {
  display: inline-block;
  padding: 0.7rem 1.5rem;
  background-color: #3fa36b;
  color: white;
  font-weight: bold;
  border: none;
  border-radius: 0.5rem;
  text-decoration: none;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.12);
  transition: background 0.2s, box-shadow 0.2s;
  cursor: pointer;
}

.download_div a:hover {
  background-color: #31905a;
  box-shadow: 0 4px 16px rgba(0, 0, 0, 0.18);
}
</style>