<script setup>
defineEmits(['navigate'])
</script>

<template>
  <header class="navbar">
    <button
        class="logo"
        @click="$emit('navigate', 'home')"
        aria-label="Zur Startseite"
    >
      <span class="brand-time">Time</span><span class="brand-core">Core</span>
    </button>

    <nav aria-label="Hauptnavigation">
      <button @click="$emit('navigate', 'features')">Features</button>
      <button @click="$emit('navigate', 'download')">Download</button>
      <button @click="$emit('navigate', 'about')">About</button>
      <button @click="$emit('navigate', 'contact')">Kontakt</button>
    </nav>
  </header>
</template>

<style scoped>
.navbar {
  position: sticky;
  top: 0;
  z-index: 10;
  background: rgba(7, 27, 51, .95);
  backdrop-filter: blur(14px);
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 18px 36px;
  border-bottom: 1px solid rgba(255,255,255,.1);
}

.logo,
nav button {
  background: none;
  border: none;
  color: white;
}

.logo {
  font-size: 1.3rem;
  font-weight: 800;
  letter-spacing: -0.02em;
}

.brand-time {
  color: #ffffff;
}

.brand-core {
  color: #14b8a6;
}

nav {
  display: flex;
  gap: 18px;
}

nav button {
  font-weight: 600;
}

@media (max-width: 760px) {
  .navbar {
    flex-direction: column;
    gap: 16px;
  }

  nav {
    flex-wrap: wrap;
    justify-content: center;
  }
}
</style>