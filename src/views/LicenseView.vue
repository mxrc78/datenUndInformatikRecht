<template>
  <section class="section license-page">

    <div class="license-hero">
      <p class="eyebrow">Rechtliches</p>

      <h1>Lizenzbedingungen</h1>

      <p>
        Diese Seite beschreibt die Nutzungsrechte für TimeCore,
        verbleibende Rechte am Produkt, untersagte Nutzungen,
        Haftungsbeschränkungen sowie Bildnachweise und verwendete KI-Tools.
      </p>
    </div>

    <div class="license-layout">

      <article class="card main-license">
        <h2>Lizenzbedingungen & Verbleibende Rechte</h2>

        <p>
          Nutzer, die eine Lizenz erwerben, erhalten das Recht, TimeCore zu installieren und zu verwenden sowie Updates herunterzuladen. Alle Rechte an der Software verbleiben bei TimeCore.
        </p>





        <div class="license-columns">

          <div>
            <h3>Verbleibende Rechte</h3>

            <ul>
              <li>Sämtliche Urheberrechte</li>
              <li>Markenrechte und Designrechte</li>
              <li>Rechte am Quellcode</li>
              <li>Rechte an Benutzeroberflächen und Grafiken</li>
              <li>Rechte an Dokumentationen und digitalen Inhalten</li>
            </ul>
          </div>

          <div>
            <h3>Untersagte Nutzung</h3>

            <ul>
              <li>Weiterverkauf der Software</li>
              <li>Unerlaubtes Kopieren oder Weitergeben</li>
              <li>Veränderung des Quellcodes</li>


              <li>Unerlaubte Verwendung von Marken oder Designs</li>
            </ul>
          </div>

        </div>
      </article>
      <article class="card liability-card">
        <h2>Haftungsbeschränkung</h2>



        <p>
          TimeCore übernimmt keine Haftung für direkte oder indirekte Schäden,
          Datenverluste oder sonstige
          Folgeschäden, die durch die Nutzung Software entstehen.
        </p>

        <p>
          TimeCore haftet, soweit dies gesetzlich zulässig ist, nicht für Schäden, die durch leichte Fahrlässigkeit verursacht wurden.
        </p>

        <p>
          Nutzer sind selbst dafür verantwortlich,
          regelmäßige Datensicherungen durchzuführen
          und geeignete Sicherheitsmaßnahmen zum Schutz ihrer Systeme
          und Daten zu treffen.
        </p>
      </article>

    </div>

    <article class="media-note">

      <div>
        <p class="eyebrow">Bildnachweise</p>

        <h2>KI-Tools & Medien</h2>
      </div>

      <p>
        Die auf dieser Website verwendeten Bilder,
        Grafiken und Markenvisualisierungen wurden mit
        <strong>OpenAI Image Generation</strong>
        erstellt und dienen ausschließlich Demonstrations-
        und Bildungszwecken.
      </p>

      <p>
        Für die Website wird die Schriftart
        <strong>Inter</strong>
        verwendet (SIL Open Font License).

      </p>

    </article>

  </section>
</template>

<style scoped>
.license-page {
  padding-top: 64px;
}

.license-hero {
  max-width: 880px;
  margin-bottom: 44px;
  padding: 36px;
  border-radius: 32px;
  background: #123252;
  box-shadow: 0 24px 60px rgba(0, 0, 0, 0.22);
  border: 1px solid rgba(255,255,255,.08);
}

.license-hero h1 {
  margin: 0 0 16px;
}

.license-hero p {
  color: #d7e3ee;
  line-height: 1.8;
  max-width: 760px;
}

.eyebrow {
  margin: 0 0 10px;
  color: #14b8a6;
  font-weight: 800;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  font-size: 0.82rem;
}

.license-layout {
  display: grid;
  grid-template-columns: 1fr;
  gap: 28px;
  align-items: start;
}

.card {
  background: #123252;
  border-radius: 30px;
  padding: 32px;
  box-shadow: 0 24px 60px rgba(0, 0, 0, 0.25);
  border: 1px solid rgba(255, 255, 255, 0.08);
}

.card h2 {
  margin-top: 0;
  color: white;
}

.card h3 {
  margin-top: 0;
  color: white;
}

.card p,
.card li,
.media-note p {
  color: #b8c7d6;
  line-height: 1.75;
}

.main-license {
  display: grid;
  gap: 22px;
}

.info-block {
  padding: 22px;
  border-radius: 22px;
  background: rgba(7, 27, 51, 0.65);
  border: 1px solid rgba(255,255,255,.08);
}

.info-block ul {
  margin-bottom: 0;
}

.warning {
  border-color: rgba(20,184,166,.35);
}

.liability-card {
  height: fit-content;
}

.media-note {
  margin-top: 32px;
  padding: 30px 32px;
  border-radius: 30px;
  background: #123252;
  border: 1px solid rgba(255,255,255,.08);
  box-shadow: 0 24px 60px rgba(0,0,0,.22);
}

.media-note h2 {
  color: white;
}

.media-note p {
  margin-bottom: 16px;
}

@media (max-width: 980px) {
  .license-layout {
    grid-template-columns: 1fr;
  }
}

@media (max-width: 620px) {
  .license-hero,
  .card,
  .media-note {
    padding: 24px;
    border-radius: 24px;
  }
  .license-columns {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 28px;
    margin-top: 28px;
  }

  .license-columns ul {
    padding-left: 20px;
  }

  @media (max-width: 760px) {
    .license-columns {
      grid-template-columns: 1fr;
    }
  }
}
</style>