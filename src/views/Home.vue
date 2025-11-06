<template>
  <div class="w-full">
    <!-- Hero Section -->
    <section class="bg-gradient-to-br from-primary to-primary-dark text-white py-16 md:py-24 text-center">
      <div class="max-w-4xl mx-auto px-4">
        <!-- Logo Placeholder -->
        <div class="mb-8">
          <div class="w-32 h-32 md:w-40 md:h-40 mx-auto bg-white/10 rounded-full flex items-center justify-center text-6xl md:text-7xl backdrop-blur-sm">
            🌾
          </div>
        </div>
        
        <h1 class="text-4xl md:text-5xl lg:text-6xl font-bold mb-6 leading-tight">
          Willkommen bei der KLJB Reicholzried
        </h1>
        <p class="text-lg md:text-xl mb-8 text-white/95 max-w-3xl mx-auto leading-relaxed">
          Katholische Landjugendbewegung - Gemeinschaft, Glaube und Engagement für unsere Region seit 1947
        </p>
        <router-link 
          to="/ueber-uns"
          class="inline-block bg-secondary hover:bg-secondary/90 text-gray-900 font-semibold px-8 py-3 rounded-full transition-all transform hover:-translate-y-1 hover:shadow-lg"
        >
          Mehr erfahren
        </router-link>
      </div>
    </section>

    <!-- About Section -->
    <section class="py-16 md:py-20 bg-gray-50">
      <div class="max-w-7xl mx-auto px-4">
        <h2 class="text-3xl md:text-4xl font-bold text-center text-primary mb-12">
          Was uns ausmacht
        </h2>
        <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
          <div class="bg-white p-8 rounded-xl shadow-md hover:shadow-xl transition-all transform hover:-translate-y-2 text-center">
            <div class="text-5xl mb-4">🤝</div>
            <h3 class="text-xl font-bold text-primary mb-3">Gemeinschaft</h3>
            <p class="text-gray-600 leading-relaxed">
              Wir sind eine lebendige Gemeinschaft junger Menschen aus Reicholzried und Umgebung.
              Gemeinsam gestalten wir Aktivitäten und fördern den Zusammenhalt.
            </p>
          </div>
          
          <div class="bg-white p-8 rounded-xl shadow-md hover:shadow-xl transition-all transform hover:-translate-y-2 text-center">
            <div class="text-5xl mb-4">✝️</div>
            <h3 class="text-xl font-bold text-primary mb-3">Glaube</h3>
            <p class="text-gray-600 leading-relaxed">
              Als katholische Jugendorganisation leben und teilen wir unseren Glauben
              in einer offenen und modernen Weise.
            </p>
          </div>
          
          <div class="bg-white p-8 rounded-xl shadow-md hover:shadow-xl transition-all transform hover:-translate-y-2 text-center">
            <div class="text-5xl mb-4">🌱</div>
            <h3 class="text-xl font-bold text-primary mb-3">Engagement</h3>
            <p class="text-gray-600 leading-relaxed">
              Wir setzen uns aktiv für unsere Gemeinde und die Umwelt ein
              und übernehmen Verantwortung für unsere Region.
            </p>
          </div>
        </div>
      </div>
    </section>

    <!-- Quick Info Section -->
    <section class="py-16 md:py-20 bg-white">
      <div class="max-w-7xl mx-auto px-4">
        <h2 class="text-3xl md:text-4xl font-bold text-center text-primary mb-12">
          Das erwartet dich
        </h2>
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6">
          <div class="text-center p-6 bg-gray-50 rounded-xl">
            <div class="text-4xl mb-3">🎉</div>
            <h4 class="font-bold text-primary mb-2">PARTY #1</h4>
            <p class="text-sm text-gray-600">Die erste große Party des Jahres im Allgäu</p>
          </div>
          <div class="text-center p-6 bg-gray-50 rounded-xl">
            <div class="text-4xl mb-3">🌳</div>
            <h4 class="font-bold text-primary mb-2">Maibaum</h4>
            <p class="text-sm text-gray-600">Traditionelles Maibaumaufstellen am 1. Mai</p>
          </div>
          <div class="text-center p-6 bg-gray-50 rounded-xl">
            <div class="text-4xl mb-3">🍷</div>
            <h4 class="font-bold text-primary mb-2">Weinfest</h4>
            <p class="text-sm text-gray-600">Gemütliches Weinfest im Herbst</p>
          </div>
          <div class="text-center p-6 bg-gray-50 rounded-xl">
            <div class="text-4xl mb-3">☀️</div>
            <h4 class="font-bold text-primary mb-2">Sonnwendfeuer</h4>
            <p class="text-sm text-gray-600">Traditionelles Feuer am 21. Juni</p>
          </div>
        </div>
      </div>
    </section>

    <!-- CTA Section -->
    <section class="py-16 md:py-20 bg-gradient-to-br from-primary to-primary-dark text-white text-center">
      <div class="max-w-4xl mx-auto px-4">
        <h2 class="text-3xl md:text-4xl font-bold mb-4">Interessiert?</h2>
        <p class="text-lg md:text-xl mb-8 text-white/95">
          Komm vorbei und lerne uns kennen! Wir freuen uns auf dich.
        </p>
        <router-link 
          to="/kontakt"
          class="inline-block bg-white hover:bg-gray-100 text-primary font-semibold px-8 py-3 rounded-full transition-all transform hover:-translate-y-1 hover:shadow-lg"
        >
          Kontakt aufnehmen
        </router-link>
      </div>
    </section>
  </div>
</template>

<script setup>
// Home component
</script>
