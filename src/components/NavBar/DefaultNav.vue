<template>
  <nav class="container">
    <div class="nav">
      <router-link to="/">
        <Github class="logo" />
      </router-link>
      <Search />
      <Links />
    </div>

    <Profile class="profile" />
  </nav>
</template>

<script setup>
import Github from "../icons/Github.vue";
import Search from "./Search.vue";
import Links from "./Link.vue";
import Profile from "./Profile.vue";
</script>

<style scoped>
.container {
  display: flex;
  align-items: center;
  padding: 0px 25px;
  background: #161b22;
}
.nav {
  display: flex;
  align-items: center;
  gap: 20px;
}

.logo {
  width: 40px;
}
.profile {
  margin-left: auto;
}
</style>
