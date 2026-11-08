<script setup lang="ts">
import TaskList from './components/TaskList.vue'
</script>

<template>
  <main>
    <header>
      <h1>StudyTasks</h1>
      <p>Dein Aufgabenplaner fürs Studium</p>
    </header>

    <TaskList />
  </main>
</template>

<style scoped>
main {
  max-width: 800px;
  margin: 40px auto;
  padding: 24px;
  font-family: Arial, sans-serif;
  color: #1e293b;
}

header {
  margin-bottom: 32px;
}

h1 {
  color: #2563eb;
  margin-bottom: 8px;
}
</style>
