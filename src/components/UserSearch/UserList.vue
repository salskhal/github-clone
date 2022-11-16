<template>
  <div>
    <div class="user-heading">
      <h3>{{ count }} users</h3>
    </div>
    <div class="user-container">
      <div v-for="(user ,index ) in userData" :key="index" class="users">
        <div class="image">
          <img src="@/assets/prof.jpeg" alt="">
        </div>
        <div>
          <div class="user-name">
            <h4>{{user.name}}</h4>
            <h4>{{user.username}}</h4>
          </div>
          <h4>{{user.bio}}</h4>
          <div class="loca-mail">
            <p>{{user.location}}</p>
            <p>{{user.email}}</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from "@vue/reactivity";

const count = ref(258);

const userData = ref([
  {
    name: "Khalid Salman-Yusuf",
    username: "salskhal",
    bio: "On the path of learning everything🤪",
    location: "Abuja, Nigeria",
    email: "",

  },
  {
    name: "wataru.sanuki",
    username: "sanukin39",
    bio: "I love HHKB.",
    location: "Tokyo, Japan",
    email: "",
  },
  {
    name: "Sanika shah",
    username: "sanu11",
    bio: "SDE 1 at Amazon | Former Software Developer @aws | Former Software Developer @DTNetwork | Former Intern @IBM",
    location: "Seattle, USA",
    email: "sanikashah1110@gmail.com",
  },
]);
</script>

<style scoped>


.user-heading{
  color: white;
  padding-bottom: 20px;
  border-bottom: 1px solid #30363d;
}

.image{
  width: 25px;
  height: 25px;
  border-radius: 50%;
  overflow: hidden;
}

.image img{
  width: 100%;
}


.user-container .users:not(:last-child){
  border-bottom: 1px solid #21262d;
}

.users{
  padding: 20px 0;
  display: flex;
  gap: 10px;
}

.user-name, .loca-mail{
  display: flex;
  gap: 10px;
}
</style>
