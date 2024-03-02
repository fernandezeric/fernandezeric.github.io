<script setup>
  import { ref } from 'vue'

  defineProps({
    msg: String,
  })

  const msgStopEaten = "Hey! Deja galletas para el resto"
  const countMaxEaten = 11

  const count = ref(0)
</script>

<template>
  <h1 v-if="count < countMaxEaten">{{ msg }}</h1>
  <h1 v-else="count >= countMaxEaten">{{ msgStopEaten }}</h1>

  <div class="card">
    <button type="button" @click="count++">Eaten Cookies {{ count }}</button>
    <p>
      <a href="https://github.com/fernandezeric" target="_blank">
        <code>fernandezeric</code>
      </a>
    </p>
  </div>

  <!-- <p>
    Check out
    <a href="https://vuejs.org/guide/quick-start.html#local" target="_blank"
      >create-vue</a
    >, the official Vue + Vite starter
  </p>
  <p>
    Install
    <a href="https://github.com/vuejs/language-tools" target="_blank">Volar</a>
    in your IDE for a better DX
  </p> -->
  <p class="read-the-docs">Eric Fernández González</p>
</template>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>
