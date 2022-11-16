<template>
  <main class="home">
    <SideBar class="sidebar" />
    <HomeContent class="content"/>
  </main>
</template>
<script setup>
import SideBar from "../components/Home/SideBar.vue";
import HomeContent from "../components/Home/Content.vue"
</script>

<style scoped>
.sidebar {
  display: none;
}

.home {
  min-height: 100vh;
}

.content{
  background: #010409;
  color: #fff;
}

@media (min-width: 768px) {
  .home {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows: 1fr;
    grid-column-gap: 0px;
    grid-row-gap: 0px;
  }
  .sidebar {
    display: block;
    grid-area: 1 / 1 / 2 / 2;
    background: #0d1117;
    border-right: 1px solid #30363d;
  }

  .content {
    grid-area: 1 / 2 / 2 / 7;
  }
}

@media (min-width: 1024px) {
  .home {
    grid-template-columns: repeat(4, 1fr);
  }
}
</style>
