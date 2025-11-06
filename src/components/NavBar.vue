<template>
  <nav class="bg-primary text-white sticky top-0 z-50 shadow-lg">
    <div class="max-w-7xl mx-auto px-4 sm:px-6">
      <div class="flex justify-between items-center h-16">
        <!-- Brand -->
        <div class="flex-shrink-0">
          <router-link to="/" class="text-xl md:text-2xl font-bold hover:opacity-90 transition-opacity">
            KLJB Reicholzried
          </router-link>
        </div>
        
        <!-- Mobile menu button -->
        <button 
          @click="toggleMenu" 
          class="md:hidden p-2 rounded-md hover:bg-primary-dark focus:outline-none focus:ring-2 focus:ring-white"
          :aria-expanded="isMenuOpen"
          aria-label="Hauptmenü"
        >
          <svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path v-if="!isMenuOpen" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
            <path v-else stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
          </svg>
        </button>
        
        <!-- Desktop menu -->
        <ul class="hidden md:flex md:space-x-8">
          <li>
            <router-link 
              to="/" 
              class="nav-link px-3 py-2 rounded-md text-sm font-medium hover:text-secondary transition-colors"
              active-class="text-secondary"
            >
              Start
            </router-link>
          </li>
          <li>
            <router-link 
              to="/ueber-uns" 
              class="nav-link px-3 py-2 rounded-md text-sm font-medium hover:text-secondary transition-colors"
              active-class="text-secondary"
            >
              Über uns
            </router-link>
          </li>
          <li>
            <router-link 
              to="/termine" 
              class="nav-link px-3 py-2 rounded-md text-sm font-medium hover:text-secondary transition-colors"
              active-class="text-secondary"
            >
              Termine
            </router-link>
          </li>
          <li>
            <router-link 
              to="/kontakt" 
              class="nav-link px-3 py-2 rounded-md text-sm font-medium hover:text-secondary transition-colors"
              active-class="text-secondary"
            >
              Kontakt
            </router-link>
          </li>
        </ul>
      </div>
    </div>
    
    <!-- Mobile menu -->
    <div 
      v-show="isMenuOpen" 
      class="md:hidden border-t border-primary-dark"
    >
      <ul class="px-2 pt-2 pb-3 space-y-1">
        <li>
          <router-link 
            to="/" 
            @click="closeMenu"
            class="block px-3 py-2 rounded-md text-base font-medium hover:bg-primary-dark transition-colors"
            active-class="bg-primary-dark text-secondary"
          >
            Start
          </router-link>
        </li>
        <li>
          <router-link 
            to="/ueber-uns" 
            @click="closeMenu"
            class="block px-3 py-2 rounded-md text-base font-medium hover:bg-primary-dark transition-colors"
            active-class="bg-primary-dark text-secondary"
          >
            Über uns
          </router-link>
        </li>
        <li>
          <router-link 
            to="/termine" 
            @click="closeMenu"
            class="block px-3 py-2 rounded-md text-base font-medium hover:bg-primary-dark transition-colors"
            active-class="bg-primary-dark text-secondary"
          >
            Termine
          </router-link>
        </li>
        <li>
          <router-link 
            to="/kontakt" 
            @click="closeMenu"
            class="block px-3 py-2 rounded-md text-base font-medium hover:bg-primary-dark transition-colors"
            active-class="bg-primary-dark text-secondary"
          >
            Kontakt
          </router-link>
        </li>
      </ul>
    </div>
  </nav>
</template>

<script setup>
import { ref } from 'vue'

const isMenuOpen = ref(false)

const toggleMenu = () => {
  isMenuOpen.value = !isMenuOpen.value
}

const closeMenu = () => {
  isMenuOpen.value = false
}
</script>
