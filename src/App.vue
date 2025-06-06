<template>
  <div class="wrapper">
    <!-- Bootstrap-style sticky nav -->
    <nav class="navbar navbar-expand-md navbar-light bg-light fixed-top shadow-sm">
      <div class="container-fluid">
        <!-- Hamburger Toggle -->
        <button class="navbar-toggler" type="button" @click="toggleMenu">
          <span class="navbar-toggler-icon"></span>
        </button>

        <!-- Navbar Links -->
        <div class="collapse navbar-collapse" :class="{ show: showMenu }">
          <ul class="navbar-nav me-auto mb-2 mb-md-0">
            <li class="nav-item" v-for="(comp, name) in components" :key="name">
              <button class="nav-link btn btn-link" @click="currentComponent = name">
                {{ name }}
              </button>
            </li>
            <li class="nav-item">
              <a
                class="nav-link"
                href="https://mvcportfolio-h3fdhzh7e9gfe2f6.canadaeast-01.azurewebsites.net/"
                target="_blank"
                rel="noopener noreferrer"
              >
                MVC Project
              </a>
            </li>
          </ul>
        </div>
      </div>
    </nav>

    <!-- Main content below the fixed navbar -->
    <div class="content-container">
      <component :is="components[currentComponent]" />
    </div>
  </div>
</template>

<script setup>
import { ref, onMounted } from 'vue'
import Resume from './components/Resume.vue'
import VueProject from './components/VueProject.vue'
import Tools from './components/Tools.vue'
import About from './components/About.vue'

const currentComponent = ref('Resume')
const showMenu = ref(false)
const isMobile = ref(window.innerWidth <= 768)

const components = {
  Resume,
  About,
  Tools,
  VueProject
}

const toggleMenu = () => {
  showMenu.value = !showMenu.value
}

onMounted(() => {
  window.addEventListener('resize', () => {
    isMobile.value = window.innerWidth <= 768
    if (!isMobile.value) showMenu.value = false
  })
})
</script>

<style>
/* Offsets the content below the fixed navbar */
.content-container {
  padding-top: 70px; /* adjust if your navbar height differs */
  padding-left: 1rem;
  padding-right: 1rem;
}
</style>
