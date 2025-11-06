<template>
  <div class="contact-page">
    <!-- Hero Section -->
    <section class="hero">
      <div class="container">
        <h1>Kontakt</h1>
        <p class="hero-subtitle">Wir freuen uns auf deine Nachricht!</p>
      </div>
    </section>

    <!-- Contact Content -->
    <section class="contact-content">
      <div class="container">
        <div class="content-grid">
          <!-- Contact Information -->
          <div class="contact-info">
            <h2>Kontaktinformationen</h2>
            
            <div class="info-block">
              <div class="icon">📍</div>
              <div class="info-text">
                <h3>Adresse</h3>
                <p>Im Winkel 24</p>
                <p>87463 Reicholzried</p>
              </div>
            </div>

            <div class="info-block">
              <div class="icon">📧</div>
              <div class="info-text">
                <h3>E-Mail</h3>
                <p>
                  <a href="mailto:kljbreicholzried@t-online.de">
                    kljbreicholzried@t-online.de
                  </a>
                </p>
              </div>
            </div>

            <div class="info-block">
              <div class="icon">📞</div>
              <div class="info-text">
                <h3>Telefon</h3>
                <p>
                  <a href="tel:+4983741354">08374 / 1354</a>
                </p>
              </div>
            </div>

            <div class="info-block">
              <div class="icon">👤</div>
              <div class="info-text">
                <h3>Vorstand</h3>
                <p><strong>Jonas Besler</strong></p>
              </div>
            </div>

            <!-- Social Media -->
            <div class="social-section">
              <h3>Folge uns auf Social Media</h3>
              <div class="social-links">
                <a href="https://www.instagram.com/kljb_reicholzried/" 
                   target="_blank" 
                   rel="noopener noreferrer" 
                   class="social-link instagram"
                   aria-label="Instagram">
                  <span class="icon">📷</span>
                  <span>@kljb_reicholzried</span>
                </a>
                <a href="https://www.facebook.com/KLJBReicholzried" 
                   target="_blank" 
                   rel="noopener noreferrer" 
                   class="social-link facebook"
                   aria-label="Facebook">
                  <span class="icon">📘</span>
                  <span>KLJB Reicholzried</span>
                </a>
              </div>
            </div>

            <!-- Youth Home Info -->
            <div class="youth-home-info">
              <h3>Jugendheim Reicholzried</h3>
              <p><strong>Bildhauerweg 3</strong></p>
              <p>87463 Reicholzried</p>
              <p class="description">
                Unser Jugendheim ist der zentrale Treffpunkt für alle unsere Aktivitäten und Veranstaltungen.
              </p>
            </div>
          </div>

          <!-- Contact Form -->
          <div class="contact-form-section">
            <h2>Schreib uns eine Nachricht</h2>
            <form @submit.prevent="handleSubmit" class="contact-form">
              <div class="form-group">
                <label for="name">Name *</label>
                <input
                  type="text"
                  id="name"
                  v-model="formData.name"
                  required
                  placeholder="Dein Name"
                />
              </div>

              <div class="form-group">
                <label for="email">E-Mail *</label>
                <input
                  type="email"
                  id="email"
                  v-model="formData.email"
                  required
                  placeholder="deine.email@beispiel.de"
                />
              </div>

              <div class="form-group">
                <label for="phone">Telefon (optional)</label>
                <input
                  type="tel"
                  id="phone"
                  v-model="formData.phone"
                  placeholder="Deine Telefonnummer"
                />
              </div>

              <div class="form-group">
                <label for="subject">Betreff *</label>
                <input
                  type="text"
                  id="subject"
                  v-model="formData.subject"
                  required
                  placeholder="Worum geht es?"
                />
              </div>

              <div class="form-group">
                <label for="message">Nachricht *</label>
                <textarea
                  id="message"
                  v-model="formData.message"
                  required
                  rows="6"
                  placeholder="Deine Nachricht an uns..."
                ></textarea>
              </div>

              <div class="form-actions">
                <button type="submit" class="submit-button" :disabled="isSubmitting">
                  {{ isSubmitting ? 'Wird gesendet...' : 'Nachricht senden' }}
                </button>
              </div>

              <div v-if="submitMessage" class="submit-message" :class="submitMessageType">
                {{ submitMessage }}
              </div>
            </form>

            <p class="form-note">
              * Pflichtfelder<br>
              <small>Hinweis: Dies ist ein Demo-Formular. Die eingegebenen Daten werden nicht tatsächlich versendet.</small>
            </p>
          </div>
        </div>
      </div>
    </section>

    <!-- Join CTA Section -->
    <section class="join-section">
      <div class="container">
        <h2>Werde Teil unserer Gemeinschaft!</h2>
        <p>
          Junge Menschen zwischen 14 und 27 Jahren sind herzlich willkommen,
          bei uns mitzumachen. Komm einfach bei einem unserer wöchentlichen Treffen vorbei
          oder kontaktiere uns für mehr Informationen.
        </p>
        <div class="join-benefits">
          <div class="benefit">
            <span class="benefit-icon">🤝</span>
            <span>Neue Freunde finden</span>
          </div>
          <div class="benefit">
            <span class="benefit-icon">🎉</span>
            <span>Tolle Events erleben</span>
          </div>
          <div class="benefit">
            <span class="benefit-icon">💪</span>
            <span>Verantwortung übernehmen</span>
          </div>
          <div class="benefit">
            <span class="benefit-icon">🌱</span>
            <span>Dorf mitgestalten</span>
          </div>
        </div>
      </div>
    </section>

    <!-- Organization Section -->
    <section class="organization-section">
      <div class="container">
        <h2>Teil einer größeren Bewegung</h2>
        <p class="org-description">
          Die KLJB Reicholzried ist Teil des KLJB Kreisverbandes Kempten im Diözesanverband Augsburg
          und gehört zur bundesweiten Katholischen Landjugendbewegung.
        </p>
        <div class="org-links">
          <a href="https://www.kljb-bayern.de" target="_blank" rel="noopener noreferrer" class="org-link">
            KLJB Bayern
          </a>
          <a href="https://kljb-augsburg.de" target="_blank" rel="noopener noreferrer" class="org-link">
            KLJB Diözesanverband Augsburg
          </a>
          <a href="https://www.kljb.org" target="_blank" rel="noopener noreferrer" class="org-link">
            KLJB Bundesverband
          </a>
        </div>
      </div>
    </section>
  </div>
</template>

<script setup>
import { ref, reactive } from 'vue'

const formData = reactive({
  name: '',
  email: '',
  phone: '',
  subject: '',
  message: ''
})

const isSubmitting = ref(false)
const submitMessage = ref('')
const submitMessageType = ref('')

const handleSubmit = () => {
  isSubmitting.value = true
  submitMessage.value = ''
  
  // Simulate form submission (Demo only)
  setTimeout(() => {
    isSubmitting.value = false
    submitMessage.value = 'Vielen Dank für deine Nachricht! Hinweis: Dies ist ein Demo-Formular, die Daten wurden nicht tatsächlich versendet.'
    submitMessageType.value = 'success'
    
    // Reset form
    formData.name = ''
    formData.email = ''
    formData.phone = ''
    formData.subject = ''
    formData.message = ''
    
    // Clear message after 8 seconds
    setTimeout(() => {
      submitMessage.value = ''
    }, 8000)
  }, 1500)
}
</script>

<style scoped>
.contact-page {
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

/* Contact Content */
.contact-content {
  padding: 4rem 0;
  background-color: var(--bg-light);
}

.content-grid {
  display: grid;
  grid-template-columns: 1fr 1.2fr;
  gap: 3rem;
  align-items: start;
}

/* Contact Info */
.contact-info {
  background-color: var(--white);
  padding: 2.5rem;
  border-radius: 12px;
  box-shadow: 0 2px 12px rgba(0, 0, 0, 0.1);
}

.contact-info h2 {
  color: var(--primary-color);
  font-size: 1.8rem;
  margin-bottom: 2rem;
}

.info-block {
  display: flex;
  gap: 1.5rem;
  margin-bottom: 2rem;
  align-items: start;
}

.info-block .icon {
  font-size: 2rem;
  flex-shrink: 0;
}

.info-text h3 {
  color: var(--primary-color);
  font-size: 1.2rem;
  margin-bottom: 0.5rem;
}

.info-text p {
  color: var(--text-light);
  line-height: 1.6;
  margin-bottom: 0.25rem;
}

.info-text a {
  color: var(--primary-color);
  transition: color 0.3s ease;
}

.info-text a:hover {
  color: var(--secondary-color);
  text-decoration: underline;
}

/* Social Media Section */
.social-section {
  margin-top: 2.5rem;
  padding-top: 2rem;
  border-top: 2px solid var(--bg-light);
}

.social-section h3 {
  color: var(--primary-color);
  font-size: 1.2rem;
  margin-bottom: 1rem;
}

.social-links {
  display: flex;
  flex-direction: column;
  gap: 1rem;
}

.social-link {
  display: flex;
  align-items: center;
  gap: 1rem;
  padding: 1rem;
  background-color: var(--bg-light);
  border-radius: 8px;
  transition: all 0.3s ease;
  color: var(--text-dark);
}

.social-link:hover {
  background-color: var(--primary-color);
  color: var(--white);
  transform: translateX(5px);
}

.social-link .icon {
  font-size: 1.5rem;
}

/* Youth Home Info */
.youth-home-info {
  margin-top: 2.5rem;
  padding: 1.5rem;
  background: linear-gradient(135deg, var(--bg-light) 0%, #e8e8e8 100%);
  border-radius: 8px;
  border-left: 4px solid var(--secondary-color);
}

.youth-home-info h3 {
  color: var(--primary-color);
  font-size: 1.2rem;
  margin-bottom: 0.75rem;
}

.youth-home-info p {
  color: var(--text-light);
  line-height: 1.6;
  margin-bottom: 0.25rem;
}

.youth-home-info .description {
  margin-top: 0.75rem;
  font-style: italic;
  font-size: 0.95rem;
}

/* Contact Form Section */
.contact-form-section {
  background-color: var(--white);
  padding: 2.5rem;
  border-radius: 12px;
  box-shadow: 0 2px 12px rgba(0, 0, 0, 0.1);
}

.contact-form-section h2 {
  color: var(--primary-color);
  font-size: 1.8rem;
  margin-bottom: 2rem;
}

.contact-form {
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
}

.form-group {
  display: flex;
  flex-direction: column;
}

.form-group label {
  color: var(--text-dark);
  font-weight: 600;
  margin-bottom: 0.5rem;
  font-size: 0.95rem;
}

.form-group input,
.form-group textarea {
  padding: 0.875rem;
  border: 2px solid #e0e0e0;
  border-radius: 8px;
  font-size: 1rem;
  font-family: inherit;
  transition: border-color 0.3s ease;
}

.form-group input:focus,
.form-group textarea:focus {
  outline: none;
  border-color: var(--primary-color);
}

.form-group textarea {
  resize: vertical;
  min-height: 120px;
}

.form-actions {
  margin-top: 1rem;
}

.submit-button {
  background-color: var(--primary-color);
  color: var(--white);
  padding: 1rem 2.5rem;
  font-size: 1.1rem;
  font-weight: 600;
  border: none;
  border-radius: 50px;
  cursor: pointer;
  transition: all 0.3s ease;
  width: 100%;
}

.submit-button:hover:not(:disabled) {
  background-color: #1a4a1b;
  transform: translateY(-2px);
  box-shadow: 0 4px 12px rgba(44, 95, 45, 0.3);
}

.submit-button:disabled {
  opacity: 0.7;
  cursor: not-allowed;
}

.submit-message {
  margin-top: 1.5rem;
  padding: 1rem;
  border-radius: 8px;
  text-align: center;
  font-weight: 500;
}

.submit-message.success {
  background-color: #d4edda;
  color: #155724;
  border: 1px solid #c3e6cb;
}

.submit-message.error {
  background-color: #f8d7da;
  color: #721c24;
  border: 1px solid #f5c6cb;
}

.form-note {
  margin-top: 1.5rem;
  font-size: 0.9rem;
  color: var(--text-light);
  line-height: 1.6;
}

.form-note small {
  font-size: 0.85rem;
  color: #999;
}

/* Join Section */
.join-section {
  padding: 4rem 0;
  background-color: var(--white);
  text-align: center;
}

.join-section h2 {
  color: var(--primary-color);
  font-size: 2rem;
  margin-bottom: 1rem;
}

.join-section p {
  color: var(--text-light);
  font-size: 1.1rem;
  line-height: 1.8;
  max-width: 800px;
  margin: 0 auto 2.5rem;
}

.join-benefits {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 2rem;
  max-width: 900px;
  margin: 0 auto;
}

.benefit {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 0.75rem;
}

.benefit-icon {
  font-size: 2.5rem;
}

.benefit span:last-child {
  color: var(--primary-color);
  font-weight: 600;
  font-size: 1.05rem;
}

/* Organization Section */
.organization-section {
  padding: 4rem 0;
  background: linear-gradient(135deg, var(--primary-color) 0%, #1a4a1b 100%);
  color: var(--white);
  text-align: center;
}

.organization-section h2 {
  font-size: 2rem;
  margin-bottom: 1rem;
}

.org-description {
  font-size: 1.1rem;
  line-height: 1.8;
  max-width: 700px;
  margin: 0 auto 2.5rem;
  color: rgba(255, 255, 255, 0.95);
}

.org-links {
  display: flex;
  justify-content: center;
  gap: 1.5rem;
  flex-wrap: wrap;
}

.org-link {
  background-color: rgba(255, 255, 255, 0.1);
  color: var(--white);
  padding: 0.875rem 2rem;
  border-radius: 50px;
  border: 2px solid rgba(255, 255, 255, 0.3);
  transition: all 0.3s ease;
  font-weight: 600;
}

.org-link:hover {
  background-color: var(--secondary-color);
  color: var(--text-dark);
  border-color: var(--secondary-color);
  transform: translateY(-2px);
}

/* Responsive Design */
@media (max-width: 768px) {
  .hero h1 {
    font-size: 2rem;
  }

  .hero-subtitle {
    font-size: 1.1rem;
  }

  .contact-content {
    padding: 3rem 0;
  }

  .content-grid {
    grid-template-columns: 1fr;
    gap: 2rem;
  }

  .contact-info,
  .contact-form-section {
    padding: 2rem;
  }

  .join-section,
  .organization-section {
    padding: 3rem 0;
  }

  .join-benefits {
    grid-template-columns: 1fr;
    gap: 1.5rem;
  }

  .org-links {
    flex-direction: column;
    align-items: stretch;
    max-width: 300px;
    margin: 0 auto;
  }
}
</style>
