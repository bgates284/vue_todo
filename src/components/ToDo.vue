<script setup>
import { ref, onMounted, computed, watch } from 'vue'
import '../main.css'
import axios from 'axios'

const todos = ref([]) 
const name = ref('') 
const input_content = ref('') 
const input_category = ref(null)

const todos_asc = computed(() => todos.value.sort((a,b) => a.createdAt - b.createdAt))

watch(name, (newVal) => {
	localStorage.setItem('name', newVal)
})

watch(todos, (newVal) => {
	localStorage.setItem('todos', JSON.stringify(newVal))
}, { deep: true })

const addTodo = () => {
	if (input_content.value.trim() === '' || input_category.value === null) {
		return
	}
	todos.value.push({
		content: input_content.value,
		category: input_category.value,
		done: false,
		editable: false,
		createdAt: new Date().getTime()
	})
}

const removeTodo = (todo) => {
	todos.value = todos.value.filter((t) => t !== todo)
}

onMounted(() => {
	name.value = localStorage.getItem('name') || ''
	todos.value = JSON.parse(localStorage.getItem('todos')) || []
	// axios.get('http://localhost:1337/todo/')
	// 	.then(response => name.value = response.data[0])
})
</script>

<template>
  <div class="tech-blurb">
    <p>
      This page is built using <strong>Vue 3</strong> with the <strong>Composition API</strong> for reactive state management,
      and <strong>scoped CSS</strong> for modular styling. It also uses <strong>Axios</strong> (commented out for now)
      for potential backend integration, and leverages <strong>localStorage</strong> for client-side persistence
      of the user's name and todo items.
    </p>
  </div>

  <section class="greeting">
    <h2 class="title">
      What's up, <input type="text" id="name" placeholder="Name here" v-model="name" />
    </h2>
  </section>

  <section class="create-todo">
    <h3>CREATE A TODO</h3>
    <form id="new-todo-form" @submit.prevent="addTodo">
      <h4>What's on your todo list?</h4>
      <input type="text" name="content" id="content" placeholder="e.g. make a video" v-model="input_content" />
      <h4>Pick a category</h4>
      <div class="options">
        <label>
          <input type="radio" name="category" value="business" v-model="input_category" />
          <span class="bubble business"></span>
          <div>Business</div>
        </label>
        <label>
          <input type="radio" name="category" value="personal" v-model="input_category" />
          <span class="bubble personal"></span>
          <div>Personal</div>
        </label>
      </div>
      <input type="submit" value="Add todo" />
    </form>
  </section>

  <section class="todo-list">
    <h3>TODO LIST</h3>
    <div class="list" id="todo-list">
      <div v-for="todo in todos_asc" :key="todo.createdAt" :class="`todo-item ${todo.done && 'done'}`">
        <label>
          <input type="checkbox" v-model="todo.done" />
          <span :class="`bubble ${todo.category}`"></span>
        </label>
        <div class="todo-content">
          <input type="text" v-model="todo.content" />
        </div>
        <div class="actions">
          <button class="delete" @click="removeTodo(todo)">Delete</button>
        </div>
      </div>
    </div>
  </section>
</template>

