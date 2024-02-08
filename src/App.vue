<script setup>
// import HelloWorld from './components/HelloWorld.vue'
import { ref, onMounted, computed, watch } from 'vue'

const todos = ref([])
const name = ref('')

const input_content = ref('')
const input_category = ref(null)

const todos_asc = computed(() => todos.value.sort((a, b) => {
  return a.createdAt - b.createdAt
}))

watch(name, (newVal => {
  localStorage.setItem('name', newVal)
}))

onMounted(() => {
  name.value = localStorage.getItem('name') || ''
})
</script>

<template>
  <main class = "app">
    <section class = "greeting">
      <h2 class = "title">
        What's up, <input type="text" placeholder="Name here "
        v-model = "name"/>
      </h2>
    </section>
  </main>
</template>


