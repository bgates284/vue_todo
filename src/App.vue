<script setup>
import { ref, onMounted } from 'vue'
import Resume from './components/Resume.vue'
import ToDo from './components/ToDo.vue'
import Tools from './components/Tools.vue'
import About from './components/About.vue'

// Declare variables and refs
const currentComponent = ref('About')
const showMenu = ref(false)
const isMobile = ref(window.innerWidth <= 768)

const components = {
  ToDo,
  Resume,
  Tools,
  About
}

// Function to toggle menu visibility
const toggleMenu = () => {
  showMenu.value = !showMenu.value
}

// Listen for window resize to adjust mobile state
onMounted(() => {
  window.addEventListener('resize', () => {
    isMobile.value = window.innerWidth <= 768
    if (!isMobile.value) showMenu.value = false // Close menu on larger screens
  })
})
</script>

<template>
  <div class="wrapper">
    <!-- This nav is always visible -->
    <nav class="nav-bar">
      <button class="hamburger" @click="toggleMenu" v-if="isMobile">
        ☰
      </button>
      <div class="nav-links" :class="{'active': showMenu}">
        <button @click="currentComponent = 'About'">About</button>
        <button @click="currentComponent = 'Resume'">Resume</button>
        <button @click="currentComponent = 'Tools'">Tools</button>
        <button @click="currentComponent = 'ToDo'">ToDo Vue App</button>
      </div>
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
  align-items: center;
  justify-content: space-between;
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

.hamburger {
  display: none;
  font-size: 1.5rem;
}

.nav-links {
  display: flex;
  gap: 1rem;
}

.nav-links button {
  display: block;
}

.nav-links.active {
  display: block;
}

@media (max-width: 768px) {
  .nav-links {
    display: none;
    width: 100%;
    text-align: center;
  }

  .hamburger {
    display: block;
    background: none;
    border: none;
    font-size: 2rem;
    color: #007bff;
    cursor: pointer;
  }

  .nav-links.active {
    display: block;
    padding-top: 1rem;
  }

  .nav-links button {
    width: 100%;
    padding: 1rem;
  }
}
</style>
