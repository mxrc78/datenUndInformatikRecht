<script setup>
defineProps({
  title: String,
  text: String
})
</script>

<template>
  <article class="card">
    <h3>{{ title }}</h3>
    <p>{{ text }}</p>
  </article>
</template>

<style scoped>
h3 {
  margin-top: 0;
}

p {
  color: #b8c7d6;
  line-height: 1.6;
}
</style>