<template>
  <div class="w-full">
    <!-- Hero Section with Background -->
    <section class="relative min-h-screen flex items-center justify-center overflow-hidden bg-gradient-to-br from-primary via-primary-dark to-primary">
      <!-- Animated Background Pattern -->
      <div class="absolute inset-0 z-0 opacity-10">
        <div class="absolute inset-0" style="background-image: radial-gradient(circle at 20% 50%, rgba(151, 191, 13, 0.3) 0%, transparent 50%), radial-gradient(circle at 80% 80%, rgba(151, 191, 13, 0.2) 0%, transparent 50%), radial-gradient(circle at 40% 20%, rgba(255, 255, 255, 0.1) 0%, transparent 50%);"></div>
      </div>
      
      <!-- Hero Content -->
      <div class="relative z-10 max-w-6xl mx-auto px-4 py-24 text-center">
        <!-- Modern Logo -->
        <div class="mb-8 animate-fade-in">
          <div class="w-24 h-24 md:w-32 md:h-32 mx-auto bg-white/20 backdrop-blur-md rounded-2xl flex items-center justify-center text-5xl md:text-6xl shadow-2xl border border-white/30">
            🌾
          </div>
        </div>
        
        <h1 class="text-5xl md:text-6xl lg:text-7xl font-extrabold mb-6 leading-tight text-white drop-shadow-2xl">
          Willkommen bei der<br/>
          <span class="text-secondary">KLJB Reicholzried</span>
        </h1>
        <p class="text-xl md:text-2xl mb-10 text-white/95 max-w-3xl mx-auto leading-relaxed font-light">
          Katholische Landjugendbewegung - Gemeinschaft, Glaube und Engagement für unsere Region seit 1947
        </p>
        <div class="flex flex-col sm:flex-row gap-4 justify-center">
          <router-link 
            to="/ueber-uns"
            class="inline-block bg-secondary hover:bg-secondary/90 text-gray-900 font-bold px-10 py-4 rounded-full transition-all transform hover:scale-105 hover:shadow-2xl text-lg"
          >
            Mehr erfahren
          </router-link>
          <router-link 
            to="/kontakt"
            class="inline-block bg-white/20 backdrop-blur-md hover:bg-white/30 text-white font-bold px-10 py-4 rounded-full transition-all transform hover:scale-105 border-2 border-white/50 text-lg"
          >
            Kontakt
          </router-link>
        </div>
      </div>
      
      <!-- Scroll Indicator -->
      <div class="absolute bottom-8 left-1/2 transform -translate-x-1/2 z-10 animate-bounce">
        <svg class="w-6 h-6 text-white/70" fill="none" stroke="currentColor" viewBox="0 0 24 24">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 14l-7 7m0 0l-7-7m7 7V3"></path>
        </svg>
      </div>
    </section>

    <!-- About Section with Modern Cards -->
    <section class="py-20 md:py-28 bg-white">
      <div class="max-w-7xl mx-auto px-4">
        <div class="text-center mb-16">
          <h2 class="text-4xl md:text-5xl font-extrabold text-primary mb-4">
            Was uns ausmacht
          </h2>
          <div class="w-24 h-1 bg-secondary mx-auto rounded-full"></div>
        </div>
        
        <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
          <!-- Card 1 - Community -->
          <div class="group relative bg-gradient-to-br from-white to-gray-50 p-8 rounded-2xl shadow-lg hover:shadow-2xl transition-all duration-300 transform hover:-translate-y-3 border border-gray-100 overflow-hidden">
            <div class="absolute top-0 right-0 w-32 h-32 bg-secondary/10 rounded-full -mr-16 -mt-16 group-hover:scale-150 transition-transform duration-500"></div>
            <div class="relative z-10">
              <div class="w-16 h-16 bg-gradient-to-br from-secondary to-primary rounded-2xl flex items-center justify-center text-3xl mb-6 shadow-lg">
                🤝
              </div>
              <h3 class="text-2xl font-bold text-primary mb-4">Gemeinschaft</h3>
              <p class="text-gray-600 leading-relaxed">
                Wir sind eine lebendige Gemeinschaft junger Menschen aus Reicholzried und Umgebung.
                Gemeinsam gestalten wir Aktivitäten und fördern den Zusammenhalt.
              </p>
            </div>
          </div>
          
          <!-- Card 2 - Faith -->
          <div class="group relative bg-gradient-to-br from-white to-gray-50 p-8 rounded-2xl shadow-lg hover:shadow-2xl transition-all duration-300 transform hover:-translate-y-3 border border-gray-100 overflow-hidden">
            <div class="absolute top-0 right-0 w-32 h-32 bg-secondary/10 rounded-full -mr-16 -mt-16 group-hover:scale-150 transition-transform duration-500"></div>
            <div class="relative z-10">
              <div class="w-16 h-16 bg-gradient-to-br from-secondary to-primary rounded-2xl flex items-center justify-center text-3xl mb-6 shadow-lg">
                ✝️
              </div>
              <h3 class="text-2xl font-bold text-primary mb-4">Glaube</h3>
              <p class="text-gray-600 leading-relaxed">
                Als katholische Jugendorganisation leben und teilen wir unseren Glauben
                in einer offenen und modernen Weise.
              </p>
            </div>
          </div>
          
          <!-- Card 3 - Engagement -->
          <div class="group relative bg-gradient-to-br from-white to-gray-50 p-8 rounded-2xl shadow-lg hover:shadow-2xl transition-all duration-300 transform hover:-translate-y-3 border border-gray-100 overflow-hidden">
            <div class="absolute top-0 right-0 w-32 h-32 bg-secondary/10 rounded-full -mr-16 -mt-16 group-hover:scale-150 transition-transform duration-500"></div>
            <div class="relative z-10">
              <div class="w-16 h-16 bg-gradient-to-br from-secondary to-primary rounded-2xl flex items-center justify-center text-3xl mb-6 shadow-lg">
                🌱
              </div>
              <h3 class="text-2xl font-bold text-primary mb-4">Engagement</h3>
              <p class="text-gray-600 leading-relaxed">
                Wir setzen uns aktiv für unsere Gemeinde und die Umwelt ein
                und übernehmen Verantwortung für unsere Region.
              </p>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Events Preview with Background -->
    <section class="relative py-20 md:py-28 overflow-hidden bg-gradient-to-r from-primary-dark via-primary to-primary-dark">
      <!-- Decorative Elements -->
      <div class="absolute inset-0 z-0 opacity-10">
        <div class="absolute inset-0" style="background-image: radial-gradient(circle at 30% 30%, rgba(151, 191, 13, 0.4) 0%, transparent 50%), radial-gradient(circle at 70% 70%, rgba(255, 255, 255, 0.2) 0%, transparent 50%);"></div>
      </div>
      
      <div class="relative z-10 max-w-7xl mx-auto px-4">
        <div class="text-center mb-16">
          <h2 class="text-4xl md:text-5xl font-extrabold text-white mb-4">
            Das erwartet dich
          </h2>
          <div class="w-24 h-1 bg-secondary mx-auto rounded-full"></div>
        </div>
        
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6">
          <div class="bg-white/10 backdrop-blur-md p-6 rounded-2xl border border-white/20 hover:bg-white/20 transition-all group">
            <div class="text-5xl mb-4 group-hover:scale-110 transition-transform">🎉</div>
            <h4 class="font-bold text-white text-lg mb-2">PARTY #1</h4>
            <p class="text-sm text-white/90">Die erste große Party des Jahres im Allgäu</p>
          </div>
          <div class="bg-white/10 backdrop-blur-md p-6 rounded-2xl border border-white/20 hover:bg-white/20 transition-all group">
            <div class="text-5xl mb-4 group-hover:scale-110 transition-transform">🌳</div>
            <h4 class="font-bold text-white text-lg mb-2">Maibaum</h4>
            <p class="text-sm text-white/90">Traditionelles Maibaumaufstellen am 1. Mai</p>
          </div>
          <div class="bg-white/10 backdrop-blur-md p-6 rounded-2xl border border-white/20 hover:bg-white/20 transition-all group">
            <div class="text-5xl mb-4 group-hover:scale-110 transition-transform">🍷</div>
            <h4 class="font-bold text-white text-lg mb-2">Weinfest</h4>
            <p class="text-sm text-white/90">Gemütliches Weinfest im Herbst</p>
          </div>
          <div class="bg-white/10 backdrop-blur-md p-6 rounded-2xl border border-white/20 hover:bg-white/20 transition-all group">
            <div class="text-5xl mb-4 group-hover:scale-110 transition-transform">☀️</div>
            <h4 class="font-bold text-white text-lg mb-2">Sonnwendfeuer</h4>
            <p class="text-sm text-white/90">Traditionelles Feuer am 21. Juni</p>
          </div>
        </div>
      </div>
    </section>

    <!-- Image Gallery Section -->
    <section class="py-20 md:py-28 bg-gray-50">
      <div class="max-w-7xl mx-auto px-4">
        <div class="text-center mb-16">
          <h2 class="text-4xl md:text-5xl font-extrabold text-primary mb-4">
            Unsere Gemeinschaft
          </h2>
          <div class="w-24 h-1 bg-secondary mx-auto rounded-full"></div>
        </div>
        
        <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
          <div class="relative group overflow-hidden rounded-2xl shadow-lg h-64 bg-gradient-to-br from-secondary/20 to-primary/30">
            <div class="absolute inset-0 flex items-center justify-center text-8xl opacity-20 group-hover:opacity-30 transition-opacity">
              🤝
            </div>
            <div class="absolute inset-0 bg-gradient-to-t from-primary-dark/90 to-transparent flex items-end p-6">
              <h3 class="text-white font-bold text-xl">Zusammenhalt</h3>
            </div>
          </div>
          <div class="relative group overflow-hidden rounded-2xl shadow-lg h-64 bg-gradient-to-br from-primary/30 to-secondary/20">
            <div class="absolute inset-0 flex items-center justify-center text-8xl opacity-20 group-hover:opacity-30 transition-opacity">
              🎉
            </div>
            <div class="absolute inset-0 bg-gradient-to-t from-primary-dark/90 to-transparent flex items-end p-6">
              <h3 class="text-white font-bold text-xl">Veranstaltungen</h3>
            </div>
          </div>
          <div class="relative group overflow-hidden rounded-2xl shadow-lg h-64 bg-gradient-to-br from-secondary/30 to-primary/20">
            <div class="absolute inset-0 flex items-center justify-center text-8xl opacity-20 group-hover:opacity-30 transition-opacity">
              🌱
            </div>
            <div class="absolute inset-0 bg-gradient-to-t from-primary-dark/90 to-transparent flex items-end p-6">
              <h3 class="text-white font-bold text-xl">Engagement</h3>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- CTA Section -->
    <section class="relative py-20 md:py-28 overflow-hidden">
      <!-- Background Pattern -->
      <div class="absolute inset-0 bg-gradient-to-br from-primary via-primary-dark to-primary opacity-95"></div>
      <div class="absolute inset-0 opacity-10" style="background-image: url('data:image/svg+xml,%3Csvg width=&quot;60&quot; height=&quot;60&quot; viewBox=&quot;0 0 60 60&quot; xmlns=&quot;http://www.w3.org/2000/svg&quot;%3E%3Cg fill=&quot;none&quot; fill-rule=&quot;evenodd&quot;%3E%3Cg fill=&quot;%23ffffff&quot; fill-opacity=&quot;1&quot;%3E%3Cpath d=&quot;M36 34v-4h-2v4h-4v2h4v4h2v-4h4v-2h-4zm0-30V0h-2v4h-4v2h4v4h2V6h4V4h-4zM6 34v-4H4v4H0v2h4v4h2v-4h4v-2H6zM6 4V0H4v4H0v2h4v4h2V6h4V4H6z&quot;/%3E%3C/g%3E%3C/g%3E%3C/svg%3E');"></div>
      
      <div class="relative z-10 max-w-4xl mx-auto px-4 text-center">
        <h2 class="text-4xl md:text-5xl font-extrabold text-white mb-6">Interessiert?</h2>
        <p class="text-xl md:text-2xl mb-10 text-white/95 font-light">
          Komm vorbei und lerne uns kennen! Wir freuen uns auf dich.
        </p>
        <router-link 
          to="/kontakt"
          class="inline-block bg-white hover:bg-gray-100 text-primary font-bold px-12 py-5 rounded-full transition-all transform hover:scale-105 hover:shadow-2xl text-lg"
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
