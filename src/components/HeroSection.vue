<script setup>
import dashboardImage from '../assets/dashboard-mockup.png'

defineEmits(['navigate'])
</script>

<template>
  <section class="hero">
    <div>
      <p class="badge">Digitale Zeiterfassung für Teams</p>
      <h1>TimeCore</h1>
      <p class="slogan">Intelligente Zeiterfassung für moderne Unternehmen.</p>

      <div class="actions">
        <button class="btn btn-primary" @click="$emit('navigate', 'download')">
          Download Now
        </button>
        <button class="btn btn-secondary" @click="$emit('navigate', 'home')">
          Preise ansehen
        </button>
      </div>
    </div>

    <div class="image-wrapper">
      <img
          :src="dashboardImage"
          alt="TimeCore Dashboard Oberfläche"
          class="dashboard-image"
      />
    </div>

  </section>
</template>

<style scoped>
.hero {
  min-height: 78vh;
  display: grid;
  grid-template-columns: 1.1fr .9fr;
  gap: 48px;
  align-items: center;
  max-width: 1180px;
  margin: 0 auto;
  padding: 90px 24px;
}

.badge {
  color: #14b8a6;
  font-weight: 800;
}

h1 {
  font-size: clamp(3rem, 8vw, 6rem);
  margin: 0;
}

.slogan {
  font-size: 1.4rem;
  color: #b8c7d6;
  line-height: 1.6;
}

.actions {
  margin-top: 32px;
  display: flex;
  gap: 16px;
  flex-wrap: wrap;
}

.image-wrapper {
  display: flex;
  justify-content: center;
  align-items: center;
}

.dashboard-image {
  width: 100%;
  max-width: 620px;
  border-radius: 28px;
  box-shadow: 0 30px 80px rgba(0,0,0,.35);
}

@media (max-width: 850px) {
  .hero {
    grid-template-columns: 1fr;
  }
}
</style>