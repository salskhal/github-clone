<template>
  <div>
    <ul class="">
      <li v-for="(link, index) in links" :key="index">
        <router-link :to="link.url">{{ link.name }}</router-link>
      </li>
    </ul>
  </div>
</template>

<script setup>
import { ref } from "@vue/reactivity";

const links = ref([
  {
    name: "Pulls",
    url: "/about",
  },
  {
    name: "Issues",
    url: "/issues",
  },
  {
    name: "Marketplace",
    url: "/marketplace",
  },
  {
    name: "Explore",
    url: "/explore",
  },
]);
</script>

<style scoped>
ul {
  display: flex;
  list-style: none;
  gap: 10px;
  -webkit-transition: all 0.5s ease;
  -moz-transition: all 0.5s ease;
  transition: all 0.5s ease;
  
}

a{
    text-decoration: none;
    color: white;
    font-weight: 600;
}
</style>
