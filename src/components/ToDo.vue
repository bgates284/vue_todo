<script setup>
import { ref, onMounted, computed, watch } from 'vue'
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

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Playfair+Display:wght@600&display=swap');

.greeting,
.create-todo,
.todo-list {
  padding: 1.5rem;
  max-width: 600px;
  margin: auto;
}

.greeting .title {
  font-size: 1.8rem;
  margin-bottom: 1rem;
}

.greeting input[type="text"] {
  font-size: 1rem;
  padding: 0.4rem;
  border: 1px solid #ccc;
  border-radius: 5px;
  width: 100%;
  max-width: 300px;
}

.create-todo h3,
.todo-list h3 {
  font-size: 1.4rem;
  margin-bottom: 0.5rem;
}

#create-todo-form input[type="text"],
#create-todo-form input[type="submit"] {
  width: 100%;
  margin-bottom: 1rem;
}

.options {
  display: flex;
  gap: 1rem;
  flex-wrap: wrap;
  margin-bottom: 1rem;
}

.options label {
  display: flex;
  align-items: center;
  gap: 0.5rem;
}

.todo-list .list {
  display: flex;
  flex-direction: column;
  gap: 1rem;
}

.todo-item {
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  justify-content: space-between;
  padding: 0.75rem;
  background-color: #f8f8f8;
  border-radius: 10px;
  box-shadow: 0 1px 3px rgba(0, 0, 0, 0.1);
}

.todo-item.done input[type="text"] {
  text-decoration: line-through;
  opacity: 0.6;
}

.todo-item label {
  display: flex;
  align-items: center;
  gap: 0.5rem;
}

.todo-content {
  flex: 1 1 60%;
  margin-top: 0.5rem;
}

.todo-content input[type="text"] {
  width: 100%;
  padding: 0.4rem;
  border: 1px solid #ccc;
  border-radius: 5px;
}

.actions {
  margin-top: 0.5rem;
}

.actions .delete {
  background: #ff4d4d;
  color: white;
  border: none;
  padding: 0.4rem 0.8rem;
  border-radius: 5px;
  cursor: pointer;
  transition: background-color 0.2s ease;
}

.actions .delete:hover {
  background-color: #cc0000;
}

.tech-blurb {
  font-family: 'Playfair Display', serif;
  background: linear-gradient(to right, #f0f0f0, #ffffff);
  border: 2px solid #dcdcdc;
  border-radius: 12px;
  padding: 1.5rem;
  margin: 1rem auto;
  max-width: 800px;
  text-align: center;
  color: #333;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.05);
}

.tech-blurb p {
  margin: 0;
  font-size: 1.1rem;
  line-height: 1.6;
}

/* Mobile Responsiveness */
@media (max-width: 600px) {
  .tech-blurb {
    padding: 1rem;
    margin: 1rem;
    max-width: 90%; /* Allow the tech blurb to use more screen space */
  }

  .tech-blurb p {
    font-size: 1rem; /* Reduce font size on mobile */
    line-height: 1.4;
  }

  .todo-item {
    flex-direction: column;
    align-items: stretch;
  }

  .todo-content {
    width: 100%;
  }

  .actions {
    align-self: flex-end;
  }

  .options {
    flex-direction: column;
  }

  .greeting .title {
    font-size: 1.5rem;
  }
}
</style>
