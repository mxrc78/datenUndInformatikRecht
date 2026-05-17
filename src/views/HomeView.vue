<script setup>
import HeroSection from '../components/HeroSection.vue'
import FeatureCard from '../components/FeatureCard.vue'
import PricingCard from '../components/PricingCard.vue'

defineEmits(['navigate'])

const features = [
  ['Arbeitszeiterfassung', 'Arbeitszeiten digital, einfach und übersichtlich erfassen.'],
  ['Projekttracking', 'Projektfortschritte, Aufgaben und Arbeitszeiten zentral verwalten.'],
  ['PDF-/CSV-Export', 'Berichte für Abrechnung und Controlling exportieren.']
]
</script>

<template>
  <HeroSection @navigate="$emit('navigate', $event)" />

  <section class="section home-section">
    <div class="section-header">
      <h2>Warum TimeCore?</h2>
      <p class="lead">
        TimeCore hilft Unternehmen, Arbeitszeiten transparent, effizient und DSGVO-bewusst zu verwalten.
      </p>
    </div>

    <div class="grid">
      <FeatureCard
          v-for="feature in features"
          :key="feature[0]"
          :title="feature[0]"
          :text="feature[1]"
      />
    </div>
  </section>

  <section class="section home-section" id="pricing">
    <div class="section-header">
      <h2>Preise</h2>
    </div>

    <div class="grid">
      <PricingCard name="Starter" price="49 €" description="Für kleine Teams und Einzelunternehmen." />
      <PricingCard name="Business" price="149 €" description="Für wachsende Unternehmen mit mehreren Projekten." />
      <PricingCard name="Enterprise" price="399 €" description="Für Organisationen mit erweiterten Anforderungen." />
    </div>
  </section>
</template>

<style scoped>
.home-section {
  padding-top: 48px;
  padding-bottom: 48px;
}

.section-header {
  margin-bottom: 28px;
}

.section-header h2 {
  margin: 0 0 12px;
}

.section-header .lead {
  margin: 0;
}
</style>