<script setup>
import { ref } from 'vue'

const sent = ref(false)
</script>

<template>
  <section class="section">
    <h1>Kontakt</h1>

    <form class="card" @submit.prevent="sent = true">
      <label for="name">Name</label>
      <input id="name" required type="text" autocomplete="name" />

      <label for="email">E-Mail</label>
      <input id="email" required type="email" autocomplete="email" />

      <label for="message">Nachricht</label>
      <textarea id="message" required rows="6"></textarea>

      <button class="btn btn-primary" type="submit">Senden</button>

      <p v-if="sent" role="status">
        Vielen Dank für Ihre Anfrage.
      </p>
    </form>
  </section>
</template>