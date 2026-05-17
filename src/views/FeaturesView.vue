<script setup>
import FeatureCard from '../components/FeatureCard.vue'

const features = [
  ['Arbeitszeiterfassung', 'Start, Pause und Ende der Arbeitszeit digital erfassen.'],
  ['Projekttracking', 'Projektfortschritte, Aufgaben und Arbeitszeiten zentral verwalten.'],
  ['PDF-/CSV-Export', 'Auswertungen für Buchhaltung und Management exportieren.'],
  ['Teamverwaltung', 'Mitarbeiter, Rollen und Teams verwalten.'],
  ['Cloud-Synchronisation', 'Synchronisierte Daten auf mehreren Geräten.'],
  ['API-Unterstützung', 'Anbindung an bestehende Unternehmenssysteme.'],
  ['DSGVO-Konformität', 'Datenschutzfreundliche Prozesse']
]
</script>

<template>
  <section class="section">
    <h1>Features</h1>
    <p class="lead">TimeCore bietet alle wichtigen Funktionen für moderne digitale Zeiterfassung.</p>

    <div class="grid">
      <FeatureCard
          v-for="feature in features"
          :key="feature[0]"
          :title="feature[0]"
          :text="feature[1]"
      />
    </div>
  </section>
</template>