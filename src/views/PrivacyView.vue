<template>
  <section class="section privacy-page">
    <div class="privacy-header">
      <h1>Datenschutzerklärung</h1>
      <p>
        Der Schutz personenbezogener Daten ist TimeCore ein wichtiges Anliegen. Personenbezogene Daten werden ausschließlich im Rahmen der gesetzlichen Bestimmungen der Datenschutz-Grundverordnung (DSGVO) verarbeitet.
      </p>
    </div>

    <div class="privacy-grid">
      <article class="privacy-card">
        <h2>Datenkategorien</h2>
        <p>
          Im Rahmen der Nutzung dieser Website können personenbezogene Daten wie
          Name, E-Mail-Adresse, Kontaktanfragen
          verarbeitet werden.
        </p>
      </article>

      <article class="privacy-card">
        <h2>Kontaktformular</h2>
        <p>
          Bei Nutzung des Kontaktformulars würden Name, E-Mail-Adresse
          und Nachricht verarbeitet werden, um die Anfrage beantworten zu können.
        </p>
      </article>

      <article class="privacy-card">
        <h2>Cookies und Analyse</h2>
        <p>
          Diese Website kann technisch notwendige Cookies verwenden,
          um grundlegende Funktionen bereitzustellen.
          Analyse- und Trackingfunktionen werden ausschließlich
          zu Demonstrationszwecken dargestellt.
        </p>
      </article>

      <article class="privacy-card wide-card">
        <h2>Downloadanfragen</h2>
        <p>
          Bei einem echten Downloadprozess könnten technische Daten wie IP-Adresse,
          Browserinformationen
          verarbeitet werden. Diese Daten würden zur Sicherheit und Fehleranakyse der Website verwendet werden.
        </p>
      </article>

      <article class="privacy-card wide-card">
        <h2>Speicherdauer und Rechte</h2>
        <p>
          Personenbezogene Daten würden nur so lange gespeichert werden, wie sie
          für den jeweiligen Zweck erforderlich sind. Nutzer:innen hätten Rechte
          auf Auskunft, Berichtigung, Löschung, Einschränkung, Datenübertragbarkeit
          und Widerspruch.
        </p>
      </article>

      <article class="privacy-card wide-card">
        <h2>Kontakt</h2>
        <p>
          TimeCore<br>
          E-Mail: support@timecore.at
        </p>
        <p class="stand">Stand: Juni 2026</p>
      </article>
    </div>
  </section>
</template>

<style scoped>
.privacy-page {
  padding-top: 56px;
}

.privacy-header {
  max-width: 760px;
  margin-bottom: 48px;
}

.privacy-header h1 {
  margin: 0 0 14px;
  font-size: clamp(2.4rem, 6vw, 4.2rem);
  line-height: 1.05;
  color: white;
}

.privacy-header p {
  color: #b8c7d6;
  line-height: 1.7;
  font-size: 1.05rem;
}

.privacy-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 26px;
}

.privacy-card {
  background: #123252;
  border: 1px solid rgba(255,255,255,.08);
  border-radius: 24px;
  padding: 28px;
  box-shadow: 0 22px 55px rgba(0,0,0,.22);
}

.privacy-card h2 {
  margin: 0 0 14px;
  color: white;
  font-size: 1.55rem;
  line-height: 1.15;
}

.privacy-card p {
  margin: 0 0 12px;
  color: #b8c7d6;
  line-height: 1.75;
}

.wide-card {
  grid-column: span 3;
}

.stand {
  margin-top: 16px;
  color: #d7e3ee;
}

@media (max-width: 1000px) {
  .privacy-grid {
    grid-template-columns: repeat(2, 1fr);
  }

  .wide-card {
    grid-column: span 2;
  }
}

@media (max-width: 700px) {
  .privacy-page {
    padding-top: 36px;
  }

  .privacy-grid {
    grid-template-columns: 1fr;
  }

  .wide-card {
    grid-column: span 1;
  }

  .privacy-card {
    padding: 24px;
  }
}
</style>