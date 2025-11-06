<template>
  <div class="events-page">
    <!-- Hero Section -->
    <section class="hero">
      <div class="container">
        <h1>Termine & Veranstaltungen</h1>
        <p class="hero-subtitle">Bleib auf dem Laufenden über unsere Events</p>
      </div>
    </section>

    <!-- Calendar Section -->
    <section class="calendar-section">
      <div class="container">
        <div class="calendar-intro">
          <h2>Unsere Veranstaltungen im Überblick</h2>
          <p>
            Hier findest du alle kommenden Termine und Veranstaltungen der KLJB Reicholzried.
            Von wöchentlichen Treffen bis zu großen Events - sei dabei!
          </p>
        </div>

        <div class="calendar-container">
          <div class="calendar-wrapper">
            <iframe
              src="https://calendar.google.com/calendar/embed?height=600&wkst=2&ctz=Europe%2FBerlin&bgcolor=%23ffffff&showTitle=0&showNav=1&showDate=1&showPrint=0&showTabs=1&showCalendars=0&mode=MONTH"
              style="border-width:0"
              frameborder="0"
              scrolling="no"
              title="KLJB Reicholzried Kalender"
            ></iframe>
          </div>
          <p class="calendar-note">
            📅 Tipp: Du kannst den Kalender durchblättern und auf einzelne Termine klicken, um mehr Informationen zu erhalten.
          </p>
        </div>
      </div>
    </section>

    <!-- Regular Events Section -->
    <section class="regular-events">
      <div class="container">
        <h2>Regelmäßige Aktivitäten</h2>
        <div class="events-grid">
          <div class="event-card">
            <div class="event-icon">📅</div>
            <h3>Wöchentliche Treffen</h3>
            <p>Wir treffen uns mindestens einmal in der Woche zu gemeinsamen Aktivitäten, Spieleabenden und Planung unserer Events.</p>
          </div>

          <div class="event-card">
            <div class="event-icon">🎅</div>
            <h3>Nikolausbesuche</h3>
            <p>Am 6. Dezember besuchen wir als KLJB die Familien in Reicholzried und bringen den Nikolaus zu den Kindern.</p>
          </div>

          <div class="event-card">
            <div class="event-icon">🎄</div>
            <h3>Adventssingen</h3>
            <p>Die KLJB nimmt am Adventssingen teil, das vom Pfarrgemeinderat in der Pfarrkirche Reicholzried organisiert wird.</p>
          </div>

          <div class="event-card">
            <div class="event-icon">🎵</div>
            <h3>Seniorensingen</h3>
            <p>Beim traditionellen Seniorensingen sammeln wir für einen guten Zweck und bringen Freude zu unseren älteren Mitbürgern.</p>
          </div>
        </div>
      </div>
    </section>

    <!-- Annual Highlights -->
    <section class="annual-highlights">
      <div class="container">
        <h2>Jahreshighlights</h2>
        <div class="highlights-timeline">
          <div class="highlight-item">
            <div class="month">Januar</div>
            <div class="highlight-content">
              <h3>🎉 PARTY #1</h3>
              <p><strong>Reithalle Dietmannsried</strong></p>
              <p>Die erste große Party des Jahres im Allgäu! Mit hochkarätigen DJs und Acts feiern wir den Start ins neue Jahr. 2025 feierten wir unser zehnjähriges Jubiläum!</p>
            </div>
          </div>

          <div class="highlight-item">
            <div class="month">Februar</div>
            <div class="highlight-content">
              <h3>🍺 Bockbierfest</h3>
              <p><strong>Jugendheim Reicholzried</strong></p>
              <p>Seit Anfang der 80er Jahre organisieren wir unser zünftiges Bockbierfest mit Musik, Weißwurst und Bier.</p>
            </div>
          </div>

          <div class="highlight-item">
            <div class="month">Mai</div>
            <div class="highlight-content">
              <h3>🌳 Maibaum aufstellen</h3>
              <p><strong>Vor dem Gasthaus "Rößle"</strong></p>
              <p>Traditionell am 1. Mai ab 13:00 Uhr. Mit anschließendem Maifest (Kaffee und Kuchen) und musikalischer Umrahmung durch die Musikkapelle Reicholzried.</p>
            </div>
          </div>

          <div class="highlight-item">
            <div class="month">Juni</div>
            <div class="highlight-content">
              <h3>☀️ Sonnwendfeuer</h3>
              <p><strong>Unterhalb der Kirche</strong></p>
              <p>Am 21. Juni findet das traditionelle Sonnwendfeuer statt, mit anschließender Open-Air-Party ab 21:00 Uhr.</p>
            </div>
          </div>

          <div class="highlight-item">
            <div class="month">Oktober</div>
            <div class="highlight-content">
              <h3>🍷 Weinfest</h3>
              <p><strong>Jugendheim Reicholzried</strong></p>
              <p>Im Herbst laden wir zum gemütlichen Weinfest ein. Ab 20:00 Uhr gibt es verschiedene Weine - von fruchtig bis kräftig, begleitet von herbstlichen Schmankerln. Ab 22:00 Uhr geht's mit Barbetrieb in die Partynacht über. Einlass ab 16 Jahren.</p>
            </div>
          </div>

          <div class="highlight-item">
            <div class="month">Sommer</div>
            <div class="highlight-content">
              <h3>🚐 Landjugendausflug</h3>
              <p><strong>Wechselnde Ziele</strong></p>
              <p>Ein Highlight jedes Jahres ist unser Landjugendausflug, der schon die unterschiedlichsten Ziele gefunden hat. Gemeinsam erkunden wir neue Orte und stärken unsere Gemeinschaft.</p>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Church Activities -->
    <section class="church-activities">
      <div class="container">
        <h2>Kirchliche Aktivitäten</h2>
        <p class="section-intro">Als katholische Jugendorganisation gestalten wir aktiv das kirchliche Leben in unserer Pfarrgemeinde mit:</p>
        <div class="activities-grid">
          <div class="activity-card">
            <div class="icon">✝️</div>
            <h4>Sebastiansandacht</h4>
            <p>Im Frühjahr</p>
          </div>
          <div class="activity-card">
            <div class="icon">🌸</div>
            <h4>Fronleichnamsaltar</h4>
            <p>Im Sommer</p>
          </div>
          <div class="activity-card">
            <div class="icon">🌾</div>
            <h4>Erntedankaltar</h4>
            <p>Im Oktober</p>
          </div>
          <div class="activity-card">
            <div class="icon">📿</div>
            <h4>Oktoberrosenkranz</h4>
            <p>Im Oktober</p>
          </div>
          <div class="activity-card">
            <div class="icon">📖</div>
            <h4>Lektorendienst</h4>
            <p>Im November</p>
          </div>
          <div class="activity-card">
            <div class="icon">⛪</div>
            <h4>Jugendgottesdienst</h4>
            <p>Regelmäßig</p>
          </div>
        </div>
      </div>
    </section>

    <!-- Contact CTA -->
    <section class="cta-section">
      <div class="container">
        <h2>Du möchtest dabei sein?</h2>
        <p>Komm einfach bei einem unserer Treffen vorbei oder melde dich bei uns!</p>
        <router-link to="/kontakt" class="cta-button">
          Kontakt aufnehmen
        </router-link>
      </div>
    </section>
  </div>
</template>

<script setup>
// Events page component
</script>

<style scoped>
.events-page {
  width: 100%;
}

/* Hero Section */
.hero {
  background: linear-gradient(135deg, var(--primary-color) 0%, #1a4a1b 100%);
  color: var(--white);
  padding: 4rem 0;
  text-align: center;
}

.hero h1 {
  font-size: 3rem;
  font-weight: 700;
  margin-bottom: 1rem;
}

.hero-subtitle {
  font-size: 1.3rem;
  color: rgba(255, 255, 255, 0.95);
}

/* Calendar Section */
.calendar-section {
  padding: 4rem 0;
  background-color: var(--white);
}

.calendar-intro {
  text-align: center;
  margin-bottom: 3rem;
}

.calendar-intro h2 {
  color: var(--primary-color);
  font-size: 2rem;
  margin-bottom: 1rem;
}

.calendar-intro p {
  color: var(--text-light);
  font-size: 1.1rem;
  max-width: 700px;
  margin: 0 auto;
  line-height: 1.7;
}

.calendar-container {
  max-width: 900px;
  margin: 0 auto;
}

.calendar-wrapper {
  position: relative;
  width: 100%;
  padding-bottom: 75%; /* 4:3 Aspect Ratio */
  border-radius: 12px;
  overflow: hidden;
  box-shadow: 0 4px 20px rgba(0, 0, 0, 0.15);
  background-color: var(--white);
}

.calendar-wrapper iframe {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}

.calendar-note {
  text-align: center;
  margin-top: 1.5rem;
  color: var(--text-light);
  font-style: italic;
}

/* Regular Events Section */
.regular-events {
  padding: 4rem 0;
  background-color: var(--bg-light);
}

.regular-events h2 {
  text-align: center;
  color: var(--primary-color);
  font-size: 2rem;
  margin-bottom: 3rem;
}

.events-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 2rem;
}

.event-card {
  background-color: var(--white);
  padding: 2rem;
  border-radius: 12px;
  box-shadow: 0 2px 12px rgba(0, 0, 0, 0.1);
  text-align: center;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.event-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 4px 20px rgba(0, 0, 0, 0.15);
}

.event-icon {
  font-size: 3rem;
  margin-bottom: 1rem;
}

.event-card h3 {
  color: var(--primary-color);
  font-size: 1.3rem;
  margin-bottom: 1rem;
}

.event-card p {
  color: var(--text-light);
  line-height: 1.7;
}

/* Annual Highlights */
.annual-highlights {
  padding: 4rem 0;
  background-color: var(--white);
}

.annual-highlights h2 {
  text-align: center;
  color: var(--primary-color);
  font-size: 2rem;
  margin-bottom: 3rem;
}

.highlights-timeline {
  max-width: 900px;
  margin: 0 auto;
}

.highlight-item {
  display: grid;
  grid-template-columns: 120px 1fr;
  gap: 2rem;
  margin-bottom: 3rem;
  align-items: start;
}

.month {
  background: linear-gradient(135deg, var(--primary-color) 0%, #1a4a1b 100%);
  color: var(--white);
  padding: 1rem;
  border-radius: 12px;
  text-align: center;
  font-weight: 700;
  font-size: 1.1rem;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.15);
}

.highlight-content {
  background-color: var(--bg-light);
  padding: 2rem;
  border-radius: 12px;
  border-left: 4px solid var(--secondary-color);
}

.highlight-content h3 {
  color: var(--primary-color);
  font-size: 1.5rem;
  margin-bottom: 0.5rem;
}

.highlight-content p {
  color: var(--text-light);
  line-height: 1.7;
  margin-bottom: 0.5rem;
}

.highlight-content p strong {
  color: var(--primary-color);
  display: block;
  margin-bottom: 0.5rem;
}

/* Church Activities */
.church-activities {
  padding: 4rem 0;
  background-color: var(--bg-light);
}

.church-activities h2 {
  text-align: center;
  color: var(--primary-color);
  font-size: 2rem;
  margin-bottom: 1rem;
}

.section-intro {
  text-align: center;
  color: var(--text-light);
  font-size: 1.1rem;
  margin-bottom: 3rem;
  max-width: 700px;
  margin-left: auto;
  margin-right: auto;
}

.activities-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 1.5rem;
  max-width: 900px;
  margin: 0 auto;
}

.activity-card {
  background-color: var(--white);
  padding: 1.5rem;
  border-radius: 12px;
  text-align: center;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.08);
  transition: transform 0.3s ease;
}

.activity-card:hover {
  transform: translateY(-3px);
}

.activity-card .icon {
  font-size: 2.5rem;
  margin-bottom: 0.75rem;
}

.activity-card h4 {
  color: var(--primary-color);
  font-size: 1.1rem;
  margin-bottom: 0.5rem;
}

.activity-card p {
  color: var(--text-light);
  font-size: 0.95rem;
}

/* CTA Section */
.cta-section {
  padding: 4rem 0;
  background: linear-gradient(135deg, var(--primary-color) 0%, #1a4a1b 100%);
  color: var(--white);
  text-align: center;
}

.cta-section h2 {
  font-size: 2.5rem;
  margin-bottom: 1rem;
}

.cta-section p {
  font-size: 1.2rem;
  margin-bottom: 2rem;
  color: rgba(255, 255, 255, 0.95);
}

.cta-button {
  display: inline-block;
  background-color: var(--secondary-color);
  color: var(--text-dark);
  padding: 1rem 2.5rem;
  font-size: 1.1rem;
  font-weight: 600;
  border-radius: 50px;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  text-decoration: none;
}

.cta-button:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 12px rgba(151, 191, 13, 0.4);
}

/* Responsive Design */
@media (max-width: 768px) {
  .hero h1 {
    font-size: 2rem;
  }

  .hero-subtitle {
    font-size: 1.1rem;
  }

  .calendar-section,
  .regular-events,
  .annual-highlights,
  .church-activities,
  .cta-section {
    padding: 3rem 0;
  }

  .calendar-intro h2,
  .regular-events h2,
  .annual-highlights h2,
  .church-activities h2 {
    font-size: 1.75rem;
  }

  .highlight-item {
    grid-template-columns: 1fr;
    gap: 1rem;
  }

  .month {
    width: fit-content;
    margin: 0 auto;
  }

  .events-grid,
  .activities-grid {
    grid-template-columns: 1fr;
    gap: 1.5rem;
  }

  .cta-section h2 {
    font-size: 2rem;
  }
}
</style>
