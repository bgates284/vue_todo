<script setup>
import { ref } from 'vue'
import Resume from './components/Resume.vue'
import ToDo from './components/ToDo.vue'
import Tools from './components/Tools.vue'
import About from './components/About.vue'

const currentComponent = ref('About')

const components = {
  ToDo,
  Resume,
  Tools,
  About
}
</script>

<template>
  <div class="wrapper">
    <!-- This nav is always visible -->
    <nav class="nav-bar">
      <button @click="currentComponent = 'About'">About</button>
      <button @click="currentComponent = 'Resume'">Resume</button>
      <button @click="currentComponent = 'Tools'">Tools</button>
      <button @click="currentComponent = 'ToDo'">ToDo Vue App</button>
    </nav>

    <!-- Only this changes -->
    <component :is="components[currentComponent]" />
  </div>
</template>

<style>
.nav-bar {
  background: #f0f0f0;
  padding: 1rem;
  display: flex;
  gap: 1rem;
  border-bottom: 1px solid #ccc;
}

.nav-bar button {
  background-color: #007bff;
  color: white;
  padding: 0.5rem 1rem;
  border: none;
  border-radius: 6px;
  cursor: pointer;
  font-weight: bold;
  transition: background-color 0.2s ease;
}

.nav-bar button:hover {
  background-color: #0056b3;
}
</style>
