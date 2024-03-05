<template>
  <!-- <h1> SOCIAL MEDIA </h1> -->
  <p class="linkRef">
      <a href="https://github.com/fernandezeric" target="_blank">
        <svgGitHub class="logo"/>
        <code>GitHub</code>
      </a>
    </p>

    <p class="linkRef">
      <a href="https://www.linkedin.com/in/eric-fern%C3%A1ndez-gonz%C3%A1lez-4bab36232/" target="_blank">
        <svgLinkedin class="logo"/>
        <code>Linkedin</code>
      </a>
    </p>
</template>

<script setup lang="ts">
  import svgGitHub from '../icons/GitHub.vue'
  import svgLinkedin from '../icons/Linkedin.vue';
</script>

<style scoped>
  .linkRef{
    font-size: 32px;
    border: 1px solid #646cff;
    border-radius: 3px;
  }
  .logo{
    padding-right: 10px;
    padding-top: 10px;
  }
  .logo:hover {
    filter: drop-shadow(0 0 2em #646cffaa);
  }
</style>