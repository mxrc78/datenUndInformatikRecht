<template>
  <section class="section">
    <h1>Barrierefreiheitserklärung</h1>

    <p class="lead">
      TimeCore ist bemüht, die Website im Einklang mit den Anforderungen
      der WCAG 2.2 Konformitätsstufe AA möglichst barrierefrei zugänglich
      zu gestalten.
    </p>

    <div class="accessibility-grid">

      <article class="card">
        <h2>Geltungsbereich</h2>

        <p>
          Diese Erklärung zur Barrierefreiheit gilt für die Website
          von TimeCore sowie sämtliche dazugehörigen Unterseiten.
        </p>

        <p>
          Die Website wurde im Rahmen eines Uni-Projekts entwickelt
          und dient Demonstrationszwecken.
        </p>
      </article>

      <article class="card">
        <h2>Stand der Vereinbarkeit</h2>

        <p>
          Diese Website ist vollständig mit den Anforderungen der
          WCAG 2.2 Konformitätsstufe AA vereinbar.
        </p>

        <p>
          Bei der Entwicklung wurde insbesondere auf folgende
          Maßnahmen geachtet:
        </p>

        <ul>
          <li>semantisches HTML</li>
          <li>ausreichende Farbkontraste</li>
          <li>Tastaturbedienbarkeit</li>
          <li>responsive Darstellung</li>
        </ul>
      </article>



      <article class="card">
        <h2>Feedback & Kontakt</h2>

        <p>
          Sollten Ihnen Barrieren oder Probleme bei der Nutzung
          der Website auffallen, freuen wir uns über eine Rückmeldung.
        </p>

        <p>
          Kontakt:
          <strong>support@timecore.at</strong>
        </p>


      </article>

    </div>

    <div class="notice-card">
      <h2>Erstellung der Erklärung</h2>

      <p>
        Diese Erklärung wurde auf Grundlage einer Selbstbewertung erstellt
        und zuletzt am <strong>25. Juni 2026</strong> überprüft.
      </p>
    </div>
  </section>
</template>

<style scoped>
.accessibility-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 28px;
  margin-top: 40px;
}

.card {
  background: #123252;
  border-radius: 28px;
  padding: 30px;
  box-shadow: 0 24px 60px rgba(0,0,0,.25);
  border: 1px solid rgba(255,255,255,.08);
}

.card h2,
.notice-card h2 {
  margin-top: 0;
  color: white;
}

.card p,
.card li,
.notice-card p {
  color: #b8c7d6;
  line-height: 1.75;
}

.card li {
  margin-bottom: 10px;
}

.notice-card {
  margin-top: 32px;
  padding: 30px;
  border-radius: 28px;
  background: #123252;
  border: 1px solid rgba(255,255,255,.08);
  box-shadow: 0 24px 60px rgba(0,0,0,.22);
}

@media (max-width: 900px) {
  .accessibility-grid {
    grid-template-columns: 1fr;
  }
}
</style>