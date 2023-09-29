<script setup>
import { ref } from 'vue';

const projectsVisible = ref(false);

const showProjects = () => {
  projectsVisible.value = true;
};
</script>

<template>
  <section class="home-page" style="text-align: center; font-family: Arial, Helvetica, sans-serif;">
    <div class="intro">
      <h1>Hello and Welcome</h1>
      <p>This is my 1.3P Task Website!</p>
      <button @click="showProjects">View My Projects</button>
    </div>
    <div class="project-list" v-if="projectsVisible">
      <h2>My Projects</h2>
      <ul style="list-style-type: none;">
        <li>
          <h3>
            <a href="https://github.com/SamCairnsDeakinStudent/SIT120Tasks.git" target="_blank">Project 1</a>
          </h3>
          <p>GitHub link to Task 1</p>
        </li>
        <li>
          <h3>
            <a href="https://github.com/SamCairnsDeakinStudent/SIT120Tasks.git" target="_blank">Project 2</a>
          </h3>
          <p>GitHub link to Task 2</p>
        </li>
        <li>
          <h3>
            <a href="https://github.com/SamCairnsDeakinStudent/SIT120Tasks.git" target="_blank">Project 3</a>
          </h3>
          <p>GitHub link to Task 3</p>
        </li>
      </ul>
    </div>
  </section>
</template>
