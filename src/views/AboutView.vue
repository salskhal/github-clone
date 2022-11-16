<template>
  <div class="container">
    <div class="grid">
      <RepoUser />
      <UserList />
    </div>


    <!-- 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 -->
  </div>
</template>

<script setup>
//   token: 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

import RepoUser from "../components/UserSearch/RepoUser.vue";
import UserList from "../components/UserSearch/UserList.vue";
</script>

<style scoped>
.container {
  min-height: 100vh;
  background: #0d1117;
  padding-inline: 20px;
  padding-top: 20px;
}

.grid {
  display: grid;
  grid-template-columns: 1fr 3fr;
  justify-content: center;
  align-items: flex-start;
  gap: 20px;
}



@media (min-width: 768px) {
  .container {
    padding-inline: 20px;
  }
}
@media (min-width: 1024px) {
  .container {
    padding-inline: 300px;
  }
}
</style>
