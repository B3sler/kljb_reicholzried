<template>
  <nav class="navbar">
    <div class="container nav-container">
      <div class="nav-brand">
        <router-link to="/" class="brand-link">
          <h1>KLJB Reicholzried</h1>
        </router-link>
      </div>
      
      <button class="nav-toggle" @click="toggleMenu" :aria-expanded="isMenuOpen">
        <span></span>
        <span></span>
        <span></span>
      </button>
      
      <ul class="nav-menu" :class="{ 'active': isMenuOpen }">
        <li class="nav-item">
          <router-link to="/" class="nav-link" @click="closeMenu">
            Startseite
          </router-link>
        </li>
        <li class="nav-item">
          <a href="#" class="nav-link" @click="closeMenu">
            Über uns
          </a>
        </li>
        <li class="nav-item">
          <a href="#" class="nav-link" @click="closeMenu">
            Veranstaltungen
          </a>
        </li>
        <li class="nav-item">
          <a href="#" class="nav-link" @click="closeMenu">
            Kontakt
          </a>
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

<style scoped>
.navbar {
  background-color: var(--primary-color);
  color: var(--white);
  padding: 1rem 0;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  position: sticky;
  top: 0;
  z-index: 100;
}

.nav-container {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.nav-brand h1 {
  font-size: 1.5rem;
  font-weight: 700;
  color: var(--white);
}

.brand-link {
  transition: opacity 0.3s ease;
}

.brand-link:hover {
  opacity: 0.9;
}

.nav-toggle {
  display: none;
  flex-direction: column;
  background: none;
  border: none;
  cursor: pointer;
  padding: 0.5rem;
}

.nav-toggle span {
  width: 25px;
  height: 3px;
  background-color: var(--white);
  margin: 3px 0;
  transition: 0.3s;
  border-radius: 3px;
}

.nav-menu {
  display: flex;
  gap: 2rem;
  align-items: center;
}

.nav-item {
  position: relative;
}

.nav-link {
  color: var(--white);
  font-size: 1rem;
  font-weight: 500;
  padding: 0.5rem 0;
  transition: color 0.3s ease;
  display: block;
}

.nav-link:hover {
  color: var(--secondary-color);
}

.nav-link::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: 0;
  width: 0;
  height: 2px;
  background-color: var(--secondary-color);
  transition: width 0.3s ease;
}

.nav-link:hover::after {
  width: 100%;
}

.router-link-active {
  color: var(--secondary-color);
}

@media (max-width: 768px) {
  .nav-toggle {
    display: flex;
  }
  
  .nav-menu {
    position: absolute;
    top: 100%;
    left: 0;
    right: 0;
    background-color: var(--primary-color);
    flex-direction: column;
    gap: 0;
    padding: 1rem 0;
    max-height: 0;
    overflow: hidden;
    transition: max-height 0.3s ease;
  }
  
  .nav-menu.active {
    max-height: 400px;
  }
  
  .nav-item {
    width: 100%;
    text-align: center;
  }
  
  .nav-link {
    padding: 1rem;
  }
  
  .nav-link::after {
    display: none;
  }
}
</style>
