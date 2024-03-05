<script setup>
  import { ref } from 'vue'
  import SocialMedia from './SocialMedia.vue';

  defineProps({
    msg: String,
  })

  const msgStopEaten = "Hey! i wanna cookies too"
  const countMaxEaten = 11

  const count = ref(0)
</script>

<template>
  <h1 v-if="count < countMaxEaten">{{ msg }}</h1>
  <h1 v-else="count >= countMaxEaten">{{ msgStopEaten }}</h1>

  <div class="card">
    <button type="button" @click="count++">Eaten Cookies {{ count }}</button>
    
    <SocialMedia/>
  </div>
  <p class="read-the-docs">Eric Fernández González</p>
</template>

<style scoped>
  .read-the-docs {
    color: #888;
  }
</style>
