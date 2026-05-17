<script setup>
import wordmark from '../assets/wordmark.png'
import wortbildmarke from '../assets/wortbildmarke.png'
import bildmarke from '../assets/bildmarke.png'
import farbmarke from '../assets/farbmarke.png'
</script>

<template>
  <section class="section">
    <h1>About Us</h1>

    <p class="lead">
      TimeCore Solutions GmbH entwickelt moderne Softwarelösungen für digitale
      Zeiterfassung, Projekttracking und effiziente Teamorganisation.
    </p>

    <div class="company-card">
      <h2>TimeCore</h2>

      <p><strong>Standort:</strong> Wien, Österreich</p>
      <p><strong>Mitarbeiter:</strong> 6</p>
      <p>
        <strong>Mission:</strong>
        Moderne und effiziente digitale Zeiterfassung für Unternehmen und Teams.
      </p>
    </div>

    <h2 class="subheading">Unsere Markenformen</h2>

    <div class="brand-grid">
      <article class="brand-card">
        <img
            :src="wordmark"
            alt="TimeCore Wortmarke"
            class="brand-image"
        />

        <h3>Wortmarke</h3>

        <p>
          Die Wortmarke „TimeCore“ repräsentiert die digitale Identität der
          Software. Der Name kombiniert „Time“ für Zeit und „Core“ für ein
          zentrales System.
        </p>
      </article>

      <article class="brand-card">
        <img
            :src="wortbildmarke"
            alt="TimeCore Wortbildmarke mit Uhrsymbol"
            class="brand-image"
        />

        <h3>Wortbildmarke</h3>

        <p>
          Die Wortbildmarke kombiniert den Schriftzug „TimeCore“ mit dem
          minimalistischen Uhrsymbol. Sie bildet die primäre visuelle
          Unternehmensidentität.
        </p>

        <p>
        </p>
      </article>

      <article class="brand-card">
        <img
            :src="bildmarke"
            alt="TimeCore Bildmarke als minimalistisches Uhrsymbol"
            class="brand-image"
        />

        <h3>Bildmarke</h3>

        <p>
          Die Bildmarke besteht aus einem reduzierten Uhrsymbol. Sie steht für
          Zeit und Struktur.
        </p>

        <p>
          Sie kann unabhängig vom Schriftzug verwendet werden, zum Beispiel als
          App-Icon, Favicon, Symbol in der Navigation oder auf Downloadbuttons.
        </p>
      </article>

      <article class="brand-card">
        <img
            :src="farbmarke"
            alt="TimeCore Farbmarke mit Dunkelblau und Türkis"
            class="brand-image"
        />

        <h3>Farbmarke</h3>

        <p>
          Die Farbmarke basiert auf den Unternehmensfarben Dunkelblau
          <strong>#071B33</strong> und Türkis <strong>#14B8A6</strong>.
        </p>

        <p>
          Dunkelblau steht für Vertrauen, Sicherheit und Professionalität.
          Türkis symbolisiert Innovation, digitale Technologie und Effizienz.
        </p>
      </article>
    </div>

    <div class="legal-grid">
      <article class="card">
        <h2>Nizza-Klassen</h2>

        <p>
          Die Marken von TimeCore werden den passenden Nizza-Klassen für
          Softwareprodukte, Unternehmensorganisation und digitale
          Dienstleistungen zugeordnet.
        </p>

        <ul>
          <li>
            <strong>Klasse 9:</strong>
            Herunterladbare Software, Computerprogramme und mobile Anwendungen.
          </li>

          <li>
            <strong>Klasse 35:</strong>
            Büroarbeiten, Geschäftsführung, Unternehmensverwaltung und
            organisatorisches Management.
          </li>

          <li>
            <strong>Klasse 42:</strong>
            Entwurf und Entwicklung von Computerhardware und Software;
            Software as a Service (SaaS); Cloud-Computing.
          </li>
        </ul>
      </article>

      <article class="card">
        <h2>Markenrechtlicher Hinweis</h2>

        <p>
          Bei der Gestaltung der Marken wurde darauf geachtet, keine bestehenden
          Markenrechte zu verletzen. Wortwahl, Bildwahl, Farbwahl, Positionswahl
          und Formwahl wurden eigenständig entwickelt.
        </p>


      </article>
    </div>
  </section>
</template>

<style scoped>
.company-card {
  margin-top: 36px;
  margin-bottom: 72px;
  padding: 34px;
  border-radius: 28px;
  background: linear-gradient(135deg, #123252, #0d2744);
  box-shadow: 0 24px 60px rgba(0, 0, 0, 0.25);
}

.company-card h2 {
  margin-top: 0;
  color: white;
}

.company-card p {
  line-height: 1.7;
}

.subheading {
  margin-bottom: 28px;
}

.brand-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 28px;
  margin-bottom: 72px;
}

.brand-card {
  background: #123252;
  border-radius: 28px;
  padding: 28px;
  box-shadow: 0 24px 60px rgba(0, 0, 0, 0.25);
  border: 1px solid rgba(255, 255, 255, 0.08);
}

.brand-image {
  width: 100%;
  height: 230px;
  object-fit: cover;
  object-position: center -70px;
  border-radius: 20px;
  margin-bottom: 24px;
  background: #071b33;
}

.brand-card h3 {
  font-size: 1.7rem;
  margin-top: 0;
  margin-bottom: 14px;
}

.brand-card p {
  color: #b8c7d6;
  line-height: 1.75;
}

.legal-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 28px;
}

.legal-grid p,
.legal-grid li {
  color: #b8c7d6;
  line-height: 1.75;
}

.legal-grid li {
  margin-bottom: 14px;
}

@media (max-width: 900px) {
  .brand-grid,
  .legal-grid {
    grid-template-columns: 1fr;
  }

  .brand-image {
    height: 200px;
  }
}
</style>