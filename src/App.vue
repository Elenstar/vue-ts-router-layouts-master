<template>
  <nav>
    <router-link to="/">Главная</router-link> |
    <router-link to="/about">О нас</router-link> |
    <router-link to="/auth">Авторизация</router-link>
  </nav>
  <main>
    <AppLayout />
  </main>
</template>

<script lang="ts" setup>
import AppLayout from '@/layouts/AppLayout.vue'

</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
