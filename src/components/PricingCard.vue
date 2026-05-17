<script setup>
defineProps({
  name: String,
  price: String,
  description: String
})
</script>

<template>
  <article class="card pricing-card">
    <h3>{{ name }}</h3>
    <p class="price">{{ price }}</p>
    <p>{{ description }}</p>
    <button class="btn btn-primary">Jetzt kaufen</button>
  </article>
</template>

<style scoped>
.pricing-card {
  display: flex;
  flex-direction: column;
  gap: 14px;
}

.price {
  font-size: 2.5rem;
  font-weight: 800;
  margin: 0;
  color: #14b8a6;
}
</style>