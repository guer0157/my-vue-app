<script setup>
import Counter from "./components/Counter.vue";
import Card from "./components/Card.vue";
</script>

<template>
  <!-- To pass things like booleans, variables and numbers use bind directive -->
  <Card name="Cesar" title="Vue Developer" v-bind:age="32" />
  <Counter>
    Here are my children
    <!-- use to pass markup or html components -->
    <!-- Using directives -->
    <template v-slot:description> Describe me</template>
    <!-- Use shorthand # -->
    <template #button-text>Reset Counter</template>
  </Counter>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
