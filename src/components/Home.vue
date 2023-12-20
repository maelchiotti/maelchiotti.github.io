<script setup lang="ts">
defineProps<{
  title: string
  subtitle: string
}>()
</script>

<template>
  <div class="greetings">
    <h1 class="green">{{ title }}</h1>
    <h3>
      {{ subtitle }}
    </h3>
    <br /><br />
    <h3>
      <a href="https://github.com/maelchiotti" target="_blank" rel="noopener">GitHub</a> |
      <a href="https://www.linkedin.com/in/maelchiotti" target="_blank" rel="noopener">LinkedIn</a>
    </h3>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  position: relative;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}
</style>
