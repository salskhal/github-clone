<template>
  <div class="profile flex">
    <span class="material-symbols-outlined icon"> notifications </span>
    <div class="flex icon">
      <span class="material-symbols-outlined"> add </span>
      <span class="material-symbols-outlined"> arrow_drop_down </span>
    </div>
    <div class="flex icon">
      <div class="profile-image">
        <img src="@/assets/prof.jpeg" alt="user" />
      </div>
      <span class="material-symbols-outlined "> arrow_drop_down </span>
    </div>
  </div>
</template>
<script setup>
</script>

<style scoped>
.profile {
  gap: 15px;
}

.profile-image{
  width: 30px;
  height: 30px;
  border-radius: 100px;
  overflow: hidden;
}

.profile-image img{
  width: 100%;
}



.icon {
  color: white;
  cursor: pointer;
}

/* Utility classes */
.flex{
  display: flex;
  align-items: center;
}
</style>
