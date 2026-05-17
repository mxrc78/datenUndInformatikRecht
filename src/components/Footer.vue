<script setup>
defineEmits(['navigate'])
</script>

<template>
  <footer class="footer">
    <p>
      <strong>
        <span class="brand-time">Time</span><span class="brand-core">Core</span>
      </strong>
      · Wien, Österreich
    </p>

    <div>
      <button @click="$emit('navigate', 'license')">Lizenz</button>
      <button @click="$emit('navigate', 'privacy')">Datenschutz</button>
      <button @click="$emit('navigate', 'imprint')">Impressum</button>
      <button @click="$emit('navigate', 'accessibility')">Barrierefreiheit</button>
    </div>


  </footer>
</template>

<style scoped>
.footer {
  background: #051426;
  text-align: center;
  padding: 42px 20px;
}

.brand-time {
  color: #ffffff;
}

.brand-core {
  color: #14b8a6;
}

button {
  margin: 8px;
  color: white;
  background: none;
  border: none;
  text-decoration: underline;
}

.small {
  color: #b8c7d6;
}
</style>