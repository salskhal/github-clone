<template>
  <div>
    <ul class="lists">
      <li v-for="(link, index) in links" :key="index" class="list">
        <div class="profile-image">
          <img src="@/assets/prof.jpeg" alt="user" />
        </div>
        <p>{{ link.name }}</p>
      </li>
    </ul>
  </div>
</template>

<script setup>
import { ref } from "@vue/reactivity";
const path = ref("@/assets/");

const links = ref([
  {
    name: "salskhal/Portfolio",
  },
  {
    name: "salskhal/task-dash",
  },
  {
    name: "salskhal/twitter-clone",
  },
  {
    name: "salskhal/SkyBlog",
  },
  {
    name: "salskhal/todoApp",
  },
  {
    name: "salskhal/Portfolio-v2",
  },
]);
</script>

<style scoped>
.lists{
    list-style: none;
    display: flex;
    flex-direction: column;
    gap: 20px;
}

.list{
    display: flex;
    color: white;
    align-items: center;
    gap: 10px;
    -webkit-transition: all .5s ease;
    -moz-transition: all .5s ease;
    transition: all .5s ease;
    cursor: pointer;
}

.list:hover{
    text-decoration: underline;
}

.profile-image {
  width: 20px;
  height: 20px;
  border-radius: 100px;
  overflow: hidden;
}

.profile-image img {
  width: 100%;
}


</style>
