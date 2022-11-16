<template>
 <div>
  <DefaultNav class="default"/>
  <MobileNav class="mobile"/>
 </div>
</template>

<script setup>
import DefaultNav from "./DefaultNav.vue"
import MobileNav from "./MobileNav.vue"
</script>

<style scoped>


.default{
  display: none;
}

@media (min-width: 768px) {
  .default{
    display: flex;
  }
  .mobile{
    display: none;
  }
}

</style>
