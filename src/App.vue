<script setup lang="ts">
import {User,UserId} from './domain/auth/lib'
const user = User({id: UserId(crypto.randomUUID())})
</script>

<template>
  <img src="/vite-deno.svg" alt="Vite with Deno" />
  <div>
    <a href="https://vite.dev" target="_blank">
      <img src="/vite.svg" class="logo" alt="Vite logo" />
    </a>
    <a href="https://vuejs.org/" target="_blank">
      <img src="./assets/vue.svg" class="logo vue" alt="Vue logo" />
    </a>
  </div>
  <pre>{{ user }}</pre>
</template>

<style scoped>
.logo {
  object-fit: contain;
  width: 8em;
  height: 6em;
  padding: 1.5em;
  will-change: filter;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
