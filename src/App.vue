<script setup>
import data from './data.json';
console.log(data);
</script>

<template>
  <div>
    <div v-for="item in data" >
      <div>
      <input type="checkbox" v-model="item.status">
      <span>{{ item.task }}</span>
      </div>
    </div>
  </div>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
