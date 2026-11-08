<script setup lang="ts">
const tasks = [
  {
    id: 1,
    title: 'Mathe-Übungsblatt bearbeiten',
    description: 'Aufgaben 1 bis 4 lösen.',
    dueDate: '2026-11-12',
    completed: false,
  },
  {
    id: 2,
    title: 'Milestone 2 vorbereiten',
    description: 'Vue-Komponente erstellen und auf GitHub hochladen.',
    dueDate: '2026-11-15',
    completed: false,
  },
  {
    id: 3,
    title: 'Projektidee festlegen',
    description: 'StudyTasks als Aufgabenplaner auswählen.',
    dueDate: '2026-10-16',
    completed: true,
  },
]
</script>

<template>
  <section>
    <h2>Meine Aufgaben</h2>

    <ul class="task-list">
      <li v-for="task in tasks" :key="task.id" class="task">
        <h3>{{ task.title }}</h3>
        <p>{{ task.description }}</p>
        <p>Abgabedatum: {{ task.dueDate }}</p>
        <span :class="{ completed: task.completed }">
          {{ task.completed ? 'Erledigt' : 'Offen' }}
        </span>
      </li>
    </ul>
  </section>
</template>

<style scoped>
.task-list {
  list-style: none;
  padding: 0;
  display: grid;
  gap: 16px;
}

.task {
  padding: 20px;
  border: 1px solid #dbe2ea;
  border-radius: 12px;
  background: white;
}

h3 {
  margin-top: 0;
}

span {
  display: inline-block;
  padding: 4px 12px;
  border-radius: 20px;
  background: #fff0cc;
  color: #704900;
}

.completed {
  background: #dcfce7;
  color: #166534;
}
</style>
