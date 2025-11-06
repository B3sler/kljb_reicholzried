<template>
  <footer class="bg-primary text-white mt-auto">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 py-12">
      <div class="grid grid-cols-1 md:grid-cols-3 gap-8 mb-8">
        <!-- About Section -->
        <div>
          <h3 class="text-xl font-bold mb-3 text-secondary">KLJB Reicholzried</h3>
          <p class="text-white/90">Katholische Landjugendbewegung</p>
          <p class="text-white/90 mt-2">Seit 1947 in Reicholzried</p>
        </div>
        
        <!-- Contact Section -->
        <div>
          <h4 class="text-lg font-semibold mb-3 text-secondary">Kontakt</h4>
          <p class="text-white/90 mb-1">Im Winkel 24</p>
          <p class="text-white/90 mb-1">87463 Reicholzried</p>
          <p class="text-white/90 mb-1">
            <a href="mailto:kljbreicholzried@t-online.de" class="hover:text-secondary transition-colors">
              kljbreicholzried@t-online.de
            </a>
          </p>
          <p class="text-white/90">
            <a href="tel:+4983741354" class="hover:text-secondary transition-colors">
              08374 / 1354
            </a>
          </p>
        </div>
        
        <!-- Social Section -->
        <div>
          <h4 class="text-lg font-semibold mb-3 text-secondary">Folge uns</h4>
          <div class="flex space-x-3">
            <a 
              href="https://www.facebook.com/KLJBReicholzried" 
              target="_blank"
              rel="noopener noreferrer"
              class="w-10 h-10 bg-white/10 rounded-full flex items-center justify-center text-xl hover:bg-secondary hover:text-gray-900 transform hover:-translate-y-1 transition-all"
              aria-label="Facebook"
            >
              📘
            </a>
            <a 
              href="https://www.instagram.com/kljb_reicholzried/" 
              target="_blank"
              rel="noopener noreferrer"
              class="w-10 h-10 bg-white/10 rounded-full flex items-center justify-center text-xl hover:bg-secondary hover:text-gray-900 transform hover:-translate-y-1 transition-all"
              aria-label="Instagram"
            >
              📷
            </a>
          </div>
        </div>
      </div>
      
      <!-- Bottom Bar -->
      <div class="border-t border-white/20 pt-6 text-center text-white/80 text-sm">
        <p>&copy; {{ currentYear }} KLJB Reicholzried. Alle Rechte vorbehalten.</p>
      </div>
    </div>
  </footer>
</template>

<script setup>
import { computed } from 'vue'

const currentYear = computed(() => new Date().getFullYear())
</script>
