<script setup>
defineProps({
  show: Boolean,
  title: String
})

defineEmits(['close'])
</script>

<template>
  <div v-if="show" class="overlay" role="dialog" aria-modal="true">
    <div class="modal">
      <h2>{{ title }}</h2>
      <slot />
      <button class="btn btn-primary" @click="$emit('close')">Schließen</button>
    </div>
  </div>
</template>

<style scoped>
.overlay {
  position: fixed;
  inset: 0;
  background: rgba(0,0,0,.7);
  display: grid;
  place-items: center;
  padding: 20px;
}

.modal {
  background: #123252;
  padding: 32px;
  border-radius: 24px;
  max-width: 520px;
}
</style>