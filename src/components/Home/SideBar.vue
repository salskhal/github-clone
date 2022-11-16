<template>
  <div class="container">
    <!-- recent -->
    <div class="repo">
      <h4>Recent Repositories</h4>
      <div class="new">
        <p>New</p>
        <Octicon />
      </div>
    </div>
    <input type="text" placeholder="Find a repository..." />
    <RepoList />
    <p class="more">Show more</p>
    <div >
      <h4 class="recent">Recent activity</h4>
      <div class="activity">
        <p>
          When you take actions across GitHub, we'll provide links to that
          activity here.
        </p>
      </div>
    </div>
  </div>
</template>
<script setup>
import Octicon from "../icons/Octicon.vue";
import RepoList from "./RepoList.vue";
</script>
<style scoped>
.container {
  padding: 40px 30px;
}

.repo {
  display: flex;
  justify-content: space-between;
  color: white;
}

.repo h4 {
  font-size: 14px;
}

.more{
    margin: 15px 0;
    font-size: 13px;
    color: #8b949e;
}

.recent{
    font-size: 15px;
    color: white;
    margin-bottom: 8px;
    font-weight: 600;
}


.activity{
    padding: 20px;
    border: 1px dashed #8b949e;
    border-radius: 10px;
    font-size: 14px;
    color: #8b949e;
}
.new {
  display: flex;
  align-items: center;
  gap: 2px;
  padding: 5px 15px;
  background: #2ea043;
  color: white;
  font-size: 12px;
  border-radius: 5px;
  cursor: pointer;
}



input {
  width: 100%;
  margin-top: 10px;
  padding: 5px 12px;
  color: white;
  border: 1px solid #30363d;
  background: #010409;
  border-radius: 6px;
  line-height: 20px;
  margin-bottom: 20px;
}
</style>
