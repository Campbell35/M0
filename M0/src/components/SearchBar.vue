<template>
  <div class="searchbar">
    <p>Welcome!! To My Website</p>
    <div class="searchbar__box">
      <input type="text" v-model="input" placeholder="Search teachers..." />
      <button>Search</button>
    </div>
    <div class="music teacher" v-for="teacher in filteredList()" :key="teacher">
      <p>{{ teacher }}</p>
    </div>

    <div class="name-error" v-if="input && !filteredList().length" :key="teacher">
      <p>No results found !</p>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'
let input = ref('')
const musicTeacher = []
function filteredList() {
  return musicTeacher.filter((teachers) =>
    teachers.toLowerCase().includes(input.value.toLowerCase())
  )
}
</script>
<style scoped>
.searchbar {
  height: 330px;
  padding-top: 2%;
  background-image: url('../assets/images/music.jpg');
}
.searchbar button {
  width: 19.1%;
  padding: 10px;
  background: black;
  color: white;
  font-size: 15px;
  border: 1px solid grey;
  border-left: none; /* Prevent double borders */
  cursor: pointer;
}

.searchbar input {
  padding: 10px;
  font-size: 15px;
  width: 50%;
  border: 1px solid grey;
  float: left;
  background: #f1f1f1;
}

.searchbar__box {
  padding-left: 20%;
}

.searchbar p {
  height: 70px;
  width: 2500px;
  padding-left: 20px;
  padding-bottom: 100px;
  color: azure;
  font-size: 50px;
}
</style>
