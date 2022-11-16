<template>
  <nav class="container">
    <span class="material-symbols-outlined"> menu </span>
    <router-link to="/">
      <Github class="logo" />
    </router-link>
    <span class="material-symbols-outlined"> notifications </span>
  </nav>
</template>

<script setup>
import Github from "../icons/Github.vue";
</script>

<style scoped>
.container {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0px 25px;
  background: #161b22;
}

.material-symbols-outlined{
    color: white;
}

.logo {
  width: 40px;
}
</style>
