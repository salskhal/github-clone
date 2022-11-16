<template>
  <div class="rep-container">
    <div v-for="(repo, index) in repos" :key="index" class="individual">
      <p class="reponame">
        {{ repo.name }}
      </p>
      <p class="count">

        {{ repo.amount }}
      </p>
    </div>
  </div>
</template>

<script setup>
import { ref } from "@vue/reactivity";
import { computed } from "@vue/runtime-core";

let amount = 20;
const repos = ref([
  {
    name: "Repositories",
    amount: "",
  },
  {
    name: "Code",
    amount: "",
  },
  {
    name: "Commits",
    amount: "",
  },
  {
    name: "Issues",
    amount: "",
  },
  {
    name: "Discussions",
    amount: "",
  },
  {
    name: "Packages",
    amount: "",
  },
  {
    name: "Marketplace",
    amount: "",
  },
  {
    name: "Topics",
    amount: "",
  },
  {
    name: "Wikis",
    amount: "",
  },
  {
    name: "Users",
    amount: amount,
  },
]);


</script>

<style scoped>


.rep-container {
  border: 1px solid #30363d;
  border-radius: 6px;
  color: white;
  overflow: hidden;
}

.individual {
  display: flex;
  padding: 10px 16px;
  align-items: center;
  justify-content: space-between;
  cursor: pointer;
  /* border-bottom: 1px solid ; */
}


.rep-container div:hover{
  background: #161b22;
}
.rep-container div:not(:last-child) {
  border-bottom: 1px solid #30363d;
}

.rep-container div:last-child {
  border-left: 3px solid #f78166;
  background: #161b22;
}

.reponame{
  font-size: 13px;
}

.count {
  display: inline-block;
  padding: 1px 6px;
  color: white;
  font-size: 13px;
  line-height: 1.4;
  border-radius: 5px;
  border-radius: 10px;
  background-color: #6e7681;
}
</style>
