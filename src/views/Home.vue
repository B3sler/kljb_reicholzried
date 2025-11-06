<template>
  <div class="home">
    <!-- Hero Section -->
    <section class="hero">
      <div class="container hero-content">
        <h1 class="hero-title">Willkommen bei der KLJB Reicholzried</h1>
        <p class="hero-subtitle">
          Katholische Landjugendbewegung - Gemeinschaft, Glaube und Engagement für unsere Region
        </p>
        <button class="cta-button">Mehr erfahren</button>
      </div>
    </section>

    <!-- About Section -->
    <section class="about">
      <div class="container">
        <h2 class="section-title">Über uns</h2>
        <div class="about-content">
          <div class="about-card">
            <div class="card-icon">🤝</div>
            <h3>Gemeinschaft</h3>
            <p>
              Wir sind eine lebendige Gemeinschaft junger Menschen aus Reicholzried und Umgebung.
              Gemeinsam gestalten wir Aktivitäten und fördern den Zusammenhalt.
            </p>
          </div>
          
          <div class="about-card">
            <div class="card-icon">✝️</div>
            <h3>Glaube</h3>
            <p>
              Als katholische Jugendorganisation leben und teilen wir unseren Glauben
              in einer offenen und modernen Weise.
            </p>
          </div>
          
          <div class="about-card">
            <div class="card-icon">🌱</div>
            <h3>Engagement</h3>
            <p>
              Wir setzen uns aktiv für unsere Gemeinde und die Umwelt ein
              und übernehmen Verantwortung für unsere Region.
            </p>
          </div>
        </div>
      </div>
    </section>

    <!-- Events Section Placeholder -->
    <section class="events">
      <div class="container">
        <h2 class="section-title">Veranstaltungen</h2>
        <p class="placeholder-text">
          Hier werden bald unsere kommenden Veranstaltungen und Events erscheinen.
          Schau regelmäßig vorbei für Updates!
        </p>
      </div>
    </section>

    <!-- Contact Call-to-Action -->
    <section class="contact-cta">
      <div class="container">
        <h2>Interessiert?</h2>
        <p>Komm vorbei und lerne uns kennen! Wir freuen uns auf dich.</p>
        <button class="cta-button secondary">Kontakt aufnehmen</button>
      </div>
    </section>
  </div>
</template>

<script setup>
// Home component - will be expanded with more content later
</script>

<style scoped>
.home {
  width: 100%;
}

/* Hero Section */
.hero {
  background: linear-gradient(135deg, var(--primary-color) 0%, #1a4a1b 100%);
  color: var(--white);
  padding: 6rem 0;
  text-align: center;
}

.hero-content {
  max-width: 800px;
  margin: 0 auto;
}

.hero-title {
  font-size: 3rem;
  font-weight: 700;
  margin-bottom: 1.5rem;
  line-height: 1.2;
}

.hero-subtitle {
  font-size: 1.25rem;
  margin-bottom: 2rem;
  line-height: 1.6;
  color: rgba(255, 255, 255, 0.95);
}

.cta-button {
  background-color: var(--secondary-color);
  color: var(--text-dark);
  border: none;
  padding: 1rem 2.5rem;
  font-size: 1.1rem;
  font-weight: 600;
  border-radius: 50px;
  cursor: pointer;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.cta-button:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 12px rgba(151, 191, 13, 0.4);
}

.cta-button.secondary {
  background-color: var(--white);
  color: var(--primary-color);
}

.cta-button.secondary:hover {
  box-shadow: 0 4px 12px rgba(255, 255, 255, 0.3);
}

/* About Section */
.about {
  padding: 5rem 0;
  background-color: var(--bg-light);
}

.section-title {
  text-align: center;
  font-size: 2.5rem;
  color: var(--primary-color);
  margin-bottom: 3rem;
}

.about-content {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 2rem;
}

.about-card {
  background-color: var(--white);
  padding: 2rem;
  border-radius: 12px;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  text-align: center;
}

.about-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 4px 16px rgba(0, 0, 0, 0.15);
}

.card-icon {
  font-size: 3rem;
  margin-bottom: 1rem;
}

.about-card h3 {
  color: var(--primary-color);
  font-size: 1.5rem;
  margin-bottom: 1rem;
}

.about-card p {
  color: var(--text-light);
  line-height: 1.8;
}

/* Events Section */
.events {
  padding: 5rem 0;
  background-color: var(--white);
}

.placeholder-text {
  text-align: center;
  font-size: 1.1rem;
  color: var(--text-light);
  max-width: 600px;
  margin: 0 auto;
}

/* Contact CTA Section */
.contact-cta {
  padding: 4rem 0;
  background: linear-gradient(135deg, var(--primary-color) 0%, #1a4a1b 100%);
  color: var(--white);
  text-align: center;
}

.contact-cta h2 {
  font-size: 2.5rem;
  margin-bottom: 1rem;
}

.contact-cta p {
  font-size: 1.2rem;
  margin-bottom: 2rem;
  color: rgba(255, 255, 255, 0.95);
}

/* Responsive Design */
@media (max-width: 768px) {
  .hero {
    padding: 4rem 0;
  }
  
  .hero-title {
    font-size: 2rem;
  }
  
  .hero-subtitle {
    font-size: 1.1rem;
  }
  
  .section-title {
    font-size: 2rem;
  }
  
  .about {
    padding: 3rem 0;
  }
  
  .events {
    padding: 3rem 0;
  }
  
  .contact-cta {
    padding: 3rem 0;
  }
  
  .contact-cta h2 {
    font-size: 2rem;
  }
  
  .about-content {
    grid-template-columns: 1fr;
  }
}

@media (max-width: 480px) {
  .hero-title {
    font-size: 1.75rem;
  }
  
  .cta-button {
    padding: 0.875rem 2rem;
    font-size: 1rem;
  }
}
</style>
