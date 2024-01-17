<script setup lang="ts">
import { RouterView } from 'vue-router'
</script>

<template>
  <section class="search-section">
    <p id="swar">swar<b>o</b>n</p>

    <div id="search">
      <input type="text" placeholder="What do you want to learn today? ">
      <button>Search</button>
    </div>
  </section>

  <RouterView />
</template>

<style scoped>
section.search-section {
  display: flex;
  align-items: center;
  flex-direction: column;
  justify-content: center;
  height: 100vh;
  width: 600px;
}

section.search-section > #search {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100%;
  gap: 1rem;
}

p#swar {
  margin: 3rem 0;
  font-size: 3rem;
}
p#swar > b {
  color: var(--color-swaron);
  font-weight: 700;
}

.search-section > #search input {
  width: 75%;
  max-width: 100%;
  padding: 1rem;
  border: 1px solid var(--color-swaron);
  border-radius: 5px;
  font-size: 1.2rem;
  font-weight: 500;
  outline: none;
}

.search-section > #search button {
  cursor: pointer;
  width: 25%;
  max-width: 100%;
  padding: 1rem;
  border: 4px solid var(--color-background-mute);
  border-radius: 10px;
  font-size: 1.2rem;
  font-weight: 500;
  outline: none;
  background-color: var(--color-swaron);
  transition: background-color 0.3s ease-in-out;
}

.search-section > #search button:hover {
  background-color: rgb(24, 88, 207)
}

</style>
