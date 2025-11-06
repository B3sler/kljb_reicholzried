<template>
  <footer class="footer">
    <div class="container footer-container">
      <div class="footer-content">
        <div class="footer-section">
          <h3>KLJB Reicholzried</h3>
          <p>Katholische Landjugendbewegung</p>
        </div>
        
        <div class="footer-section">
          <h4>Kontakt</h4>
          <p>Email: info@kljb-reicholzried.de</p>
          <p>Telefon: +49 (0) XXX XXXXXXX</p>
        </div>
        
        <div class="footer-section">
          <h4>Folge uns</h4>
          <div class="social-links">
            <a href="#" class="social-link" aria-label="Facebook">
              <span>📘</span>
            </a>
            <a href="#" class="social-link" aria-label="Instagram">
              <span>📷</span>
            </a>
          </div>
        </div>
      </div>
      
      <div class="footer-bottom">
        <p>&copy; {{ currentYear }} KLJB Reicholzried. Alle Rechte vorbehalten.</p>
      </div>
    </div>
  </footer>
</template>

<script setup>
import { computed } from 'vue'

const currentYear = computed(() => new Date().getFullYear())
</script>

<style scoped>
.footer {
  background-color: var(--primary-color);
  color: var(--white);
  padding: 3rem 0 1rem;
  margin-top: auto;
}

.footer-container {
  display: flex;
  flex-direction: column;
  gap: 2rem;
}

.footer-content {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 2rem;
}

.footer-section h3 {
  font-size: 1.5rem;
  margin-bottom: 0.5rem;
  color: var(--secondary-color);
}

.footer-section h4 {
  font-size: 1.1rem;
  margin-bottom: 0.75rem;
  color: var(--secondary-color);
}

.footer-section p {
  margin-bottom: 0.5rem;
  color: rgba(255, 255, 255, 0.9);
}

.social-links {
  display: flex;
  gap: 1rem;
  margin-top: 0.5rem;
}

.social-link {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 40px;
  height: 40px;
  background-color: rgba(255, 255, 255, 0.1);
  border-radius: 50%;
  transition: background-color 0.3s ease, transform 0.3s ease;
  font-size: 1.2rem;
}

.social-link:hover {
  background-color: var(--secondary-color);
  transform: translateY(-3px);
}

.footer-bottom {
  text-align: center;
  padding-top: 2rem;
  border-top: 1px solid rgba(255, 255, 255, 0.2);
  color: rgba(255, 255, 255, 0.8);
  font-size: 0.9rem;
}

@media (max-width: 768px) {
  .footer {
    padding: 2rem 0 1rem;
  }
  
  .footer-content {
    grid-template-columns: 1fr;
    gap: 1.5rem;
  }
  
  .footer-section {
    text-align: center;
  }
  
  .social-links {
    justify-content: center;
  }
}
</style>
