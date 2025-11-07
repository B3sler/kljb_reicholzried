<template>
  <div class="w-full">
    <!-- Hero Section with Modern Design -->
    <section class="relative py-20 md:py-28 overflow-hidden bg-gradient-to-br from-primary via-primary-dark to-primary">
      <div class="absolute inset-0 opacity-10">
        <div class="absolute inset-0" style="background-image: radial-gradient(circle at 20% 50%, rgba(151, 191, 13, 0.3) 0%, transparent 50%), radial-gradient(circle at 80% 80%, rgba(151, 191, 13, 0.2) 0%, transparent 50%);"></div>
      </div>
      <div class="relative z-10 max-w-4xl mx-auto px-4 text-center">
        <div class="inline-block mb-6">
          <div class="w-20 h-20 bg-white/20 backdrop-blur-md rounded-2xl flex items-center justify-center text-4xl shadow-xl border border-white/30">
            📅
          </div>
        </div>
        <h1 class="text-5xl md:text-6xl font-extrabold mb-6 text-white drop-shadow-2xl">
          Termine & Veranstaltungen
        </h1>
        <p class="text-xl md:text-2xl text-white/95 font-light">
          Bleib auf dem Laufenden über unsere Events
        </p>
      </div>
    </section>

    <!-- Google Calendar Section -->
    <section class="py-16 md:py-24 bg-white">
      <div class="max-w-6xl mx-auto px-4">
        <div class="text-center mb-12">
          <h2 class="text-4xl md:text-5xl font-extrabold text-primary mb-4">
            Unsere Veranstaltungen im Überblick
          </h2>
          <div class="w-24 h-1 bg-secondary mx-auto rounded-full mb-6"></div>
          <p class="text-gray-600 text-lg leading-relaxed max-w-3xl mx-auto">
            Hier findest du alle kommenden Termine und Veranstaltungen der KLJB Reicholzried.
            Von wöchentlichen Treffen bis zu großen Events - sei dabei!
          </p>
        </div>

        <!-- Modern Calendar Container -->
        <div class="bg-gradient-to-br from-gray-50 to-white p-4 md:p-8 rounded-2xl shadow-2xl border border-gray-100">
          <div class="relative w-full rounded-xl overflow-hidden shadow-lg" style="padding-bottom: 75%;">
            <iframe
              src="https://calendar.google.com/calendar/embed?height=600&wkst=2&ctz=Europe%2FBerlin&bgcolor=%23ffffff&showTitle=0&showNav=1&showDate=1&showPrint=0&showTabs=1&showCalendars=0&mode=MONTH&hl=de"
              class="absolute top-0 left-0 w-full h-full border-0"
              scrolling="no"
              title="KLJB Reicholzried Kalender"
            ></iframe>
          </div>
          <div class="mt-6 flex items-center justify-center gap-3 text-gray-600">
            <svg class="w-5 h-5 text-secondary" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 16h-1v-4h-1m1-4h.01M21 12a9 9 0 11-18 0 9 9 0 0118 0z"></path>
            </svg>
            <p class="text-sm italic">
              Tipp: Klicke auf einzelne Termine für mehr Informationen und Details
            </p>
          </div>
        </div>

        <!-- Quick Add to Calendar Button -->
        <div class="mt-8 text-center">
          <a 
            href="https://calendar.google.com/calendar/u/0/r?cid=CALENDAR_ID_HERE" 
            target="_blank"
            rel="noopener noreferrer"
            class="inline-flex items-center gap-2 bg-primary hover:bg-primary-dark text-white font-semibold px-8 py-4 rounded-full transition-all transform hover:scale-105 shadow-lg"
          >
            <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 4v16m8-8H4"></path>
            </svg>
            <span>Kalender abonnieren</span>
          </a>
        </div>
      </div>
    </section>

    <!-- Regular Events with Modern Cards -->
    <section class="py-16 md:py-24 bg-gray-50">
      <div class="max-w-7xl mx-auto px-4">
        <div class="text-center mb-12">
          <h2 class="text-4xl md:text-5xl font-extrabold text-primary mb-4">Regelmäßige Aktivitäten</h2>
          <div class="w-24 h-1 bg-secondary mx-auto rounded-full"></div>
        </div>
        
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6">
          <div class="group bg-white p-8 rounded-2xl shadow-lg hover:shadow-2xl transition-all transform hover:-translate-y-2 text-center border border-gray-100">
            <div class="w-20 h-20 bg-gradient-to-br from-secondary/20 to-primary/20 rounded-2xl flex items-center justify-center text-4xl mb-4 mx-auto group-hover:scale-110 transition-transform">
              📅
            </div>
            <h3 class="text-xl font-bold text-primary mb-3">Wöchentliche Treffen</h3>
            <p class="text-gray-600 leading-relaxed">Mindestens einmal pro Woche treffen wir uns zu Aktivitäten, Spieleabenden und Event-Planung.</p>
          </div>

          <div class="group bg-white p-8 rounded-2xl shadow-lg hover:shadow-2xl transition-all transform hover:-translate-y-2 text-center border border-gray-100">
            <div class="w-20 h-20 bg-gradient-to-br from-secondary/20 to-primary/20 rounded-2xl flex items-center justify-center text-4xl mb-4 mx-auto group-hover:scale-110 transition-transform">
              🎅
            </div>
            <h3 class="text-xl font-bold text-primary mb-3">Nikolausbesuche</h3>
            <p class="text-gray-600 leading-relaxed">Am 6. Dezember besuchen wir als KLJB die Familien und bringen den Nikolaus zu den Kindern.</p>
          </div>

          <div class="group bg-white p-8 rounded-2xl shadow-lg hover:shadow-2xl transition-all transform hover:-translate-y-2 text-center border border-gray-100">
            <div class="w-20 h-20 bg-gradient-to-br from-secondary/20 to-primary/20 rounded-2xl flex items-center justify-center text-4xl mb-4 mx-auto group-hover:scale-110 transition-transform">
              🎄
            </div>
            <h3 class="text-xl font-bold text-primary mb-3">Adventssingen</h3>
            <p class="text-gray-600 leading-relaxed">Wir nehmen am Adventssingen teil, organisiert vom Pfarrgemeinderat in der Pfarrkirche.</p>
          </div>

          <div class="group bg-white p-8 rounded-2xl shadow-lg hover:shadow-2xl transition-all transform hover:-translate-y-2 text-center border border-gray-100">
            <div class="w-20 h-20 bg-gradient-to-br from-secondary/20 to-primary/20 rounded-2xl flex items-center justify-center text-4xl mb-4 mx-auto group-hover:scale-110 transition-transform">
              🎵
            </div>
            <h3 class="text-xl font-bold text-primary mb-3">Seniorensingen</h3>
            <p class="text-gray-600 leading-relaxed">Beim Seniorensingen sammeln wir für einen guten Zweck und bringen Freude zu den Senioren.</p>
          </div>
        </div>
      </div>
    </section>

    <!-- Annual Highlights with Modern Design -->
    <section class="relative py-16 md:py-24 overflow-hidden bg-white">
      <div class="max-w-6xl mx-auto px-4">
        <div class="text-center mb-12">
          <h2 class="text-4xl md:text-5xl font-extrabold text-primary mb-4">Jahreshighlights</h2>
          <div class="w-24 h-1 bg-secondary mx-auto rounded-full"></div>
        </div>
        
        <div class="space-y-6">
          <div class="group flex flex-col md:flex-row gap-6 items-start bg-gradient-to-r from-gray-50 to-white p-6 rounded-2xl shadow-lg hover:shadow-xl transition-all">
            <div class="flex-shrink-0 w-full md:w-40 text-center">
              <div class="inline-block bg-gradient-to-br from-primary to-primary-dark text-white px-6 py-3 rounded-2xl font-bold shadow-md text-lg">
                Januar
              </div>
            </div>
            <div class="flex-1 border-l-4 border-secondary pl-6">
              <h3 class="text-2xl font-bold text-primary mb-2 flex items-center gap-2">
                <span class="text-3xl">🎉</span> PARTY #1
              </h3>
              <p class="font-semibold text-gray-700 mb-2">📍 Reithalle Dietmannsried</p>
              <p class="text-gray-600 leading-relaxed">Die erste große Party des Jahres im Allgäu! Mit hochkarätigen DJs und Acts feiern wir den Start ins neue Jahr. 2025 feierten wir unser zehnjähriges Jubiläum!</p>
            </div>
          </div>

          <div class="group flex flex-col md:flex-row gap-6 items-start bg-gradient-to-r from-gray-50 to-white p-6 rounded-2xl shadow-lg hover:shadow-xl transition-all">
            <div class="flex-shrink-0 w-full md:w-40 text-center">
              <div class="inline-block bg-gradient-to-br from-primary to-primary-dark text-white px-6 py-3 rounded-2xl font-bold shadow-md text-lg">
                Februar
              </div>
            </div>
            <div class="flex-1 border-l-4 border-secondary pl-6">
              <h3 class="text-2xl font-bold text-primary mb-2 flex items-center gap-2">
                <span class="text-3xl">🍺</span> Bockbierfest
              </h3>
              <p class="font-semibold text-gray-700 mb-2">📍 Jugendheim Reicholzried</p>
              <p class="text-gray-600 leading-relaxed">Seit Anfang der 80er Jahre organisieren wir unser zünftiges Bockbierfest mit Musik, Weißwurst und Bier.</p>
            </div>
          </div>

          <div class="group flex flex-col md:flex-row gap-6 items-start bg-gradient-to-r from-gray-50 to-white p-6 rounded-2xl shadow-lg hover:shadow-xl transition-all">
            <div class="flex-shrink-0 w-full md:w-40 text-center">
              <div class="inline-block bg-gradient-to-br from-primary to-primary-dark text-white px-6 py-3 rounded-2xl font-bold shadow-md text-lg">
                Mai
              </div>
            </div>
            <div class="flex-1 border-l-4 border-secondary pl-6">
              <h3 class="text-2xl font-bold text-primary mb-2 flex items-center gap-2">
                <span class="text-3xl">🌳</span> Maibaum aufstellen
              </h3>
              <p class="font-semibold text-gray-700 mb-2">📍 Vor dem Gasthaus "Rößle"</p>
              <p class="text-gray-600 leading-relaxed">Traditionell am 1. Mai ab 13:00 Uhr. Mit anschließendem Maifest (Kaffee und Kuchen) und musikalischer Umrahmung durch die Musikkapelle Reicholzried.</p>
            </div>
          </div>

          <div class="group flex flex-col md:flex-row gap-6 items-start bg-gradient-to-r from-gray-50 to-white p-6 rounded-2xl shadow-lg hover:shadow-xl transition-all">
            <div class="flex-shrink-0 w-full md:w-40 text-center">
              <div class="inline-block bg-gradient-to-br from-primary to-primary-dark text-white px-6 py-3 rounded-2xl font-bold shadow-md text-lg">
                Juni
              </div>
            </div>
            <div class="flex-1 border-l-4 border-secondary pl-6">
              <h3 class="text-2xl font-bold text-primary mb-2 flex items-center gap-2">
                <span class="text-3xl">☀️</span> Sonnwendfeuer
              </h3>
              <p class="font-semibold text-gray-700 mb-2">📍 Unterhalb der Kirche</p>
              <p class="text-gray-600 leading-relaxed">Am 21. Juni findet das traditionelle Sonnwendfeuer statt, mit anschließender Open-Air-Party ab 21:00 Uhr.</p>
            </div>
          </div>

          <div class="group flex flex-col md:flex-row gap-6 items-start bg-gradient-to-r from-gray-50 to-white p-6 rounded-2xl shadow-lg hover:shadow-xl transition-all">
            <div class="flex-shrink-0 w-full md:w-40 text-center">
              <div class="inline-block bg-gradient-to-br from-primary to-primary-dark text-white px-6 py-3 rounded-2xl font-bold shadow-md text-lg">
                Oktober
              </div>
            </div>
            <div class="flex-1 border-l-4 border-secondary pl-6">
              <h3 class="text-2xl font-bold text-primary mb-2 flex items-center gap-2">
                <span class="text-3xl">🍷</span> Weinfest
              </h3>
              <p class="font-semibold text-gray-700 mb-2">📍 Jugendheim Reicholzried</p>
              <p class="text-gray-600 leading-relaxed">Im Herbst laden wir zum gemütlichen Weinfest ein. Ab 20:00 Uhr verschiedene Weine mit herbstlichen Schmankerln. Ab 22:00 Uhr Barbetrieb und Partynacht. Einlass ab 16 Jahren.</p>
            </div>
          </div>

          <div class="group flex flex-col md:flex-row gap-6 items-start bg-gradient-to-r from-gray-50 to-white p-6 rounded-2xl shadow-lg hover:shadow-xl transition-all">
            <div class="flex-shrink-0 w-full md:w-40 text-center">
              <div class="inline-block bg-gradient-to-br from-primary to-primary-dark text-white px-6 py-3 rounded-2xl font-bold shadow-md text-lg">
                Sommer
              </div>
            </div>
            <div class="flex-1 border-l-4 border-secondary pl-6">
              <h3 class="text-2xl font-bold text-primary mb-2 flex items-center gap-2">
                <span class="text-3xl">🚐</span> Landjugendausflug
              </h3>
              <p class="font-semibold text-gray-700 mb-2">📍 Wechselnde Ziele</p>
              <p class="text-gray-600 leading-relaxed">Ein Highlight jedes Jahres ist unser Landjugendausflug. Gemeinsam erkunden wir neue Orte und stärken unsere Gemeinschaft.</p>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Church Activities -->
    <section class="py-12 md:py-16 bg-gray-50">
      <div class="max-w-6xl mx-auto px-4">
        <h2 class="text-2xl md:text-3xl font-bold text-center text-primary mb-4">Kirchliche Aktivitäten</h2>
        <p class="text-center text-gray-600 mb-8 max-w-3xl mx-auto">
          Als katholische Jugendorganisation gestalten wir aktiv das kirchliche Leben in unserer Pfarrgemeinde mit:
        </p>
        <div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-6 gap-4">
          <div class="bg-white p-4 rounded-xl text-center shadow-sm hover:shadow-md transition-shadow">
            <div class="text-3xl mb-2">✝️</div>
            <h4 class="font-bold text-primary text-sm mb-1">Sebastiansandacht</h4>
            <p class="text-gray-500 text-xs">Im Frühjahr</p>
          </div>
          <div class="bg-white p-4 rounded-xl text-center shadow-sm hover:shadow-md transition-shadow">
            <div class="text-3xl mb-2">🌸</div>
            <h4 class="font-bold text-primary text-sm mb-1">Fronleichnamsaltar</h4>
            <p class="text-gray-500 text-xs">Im Sommer</p>
          </div>
          <div class="bg-white p-4 rounded-xl text-center shadow-sm hover:shadow-md transition-shadow">
            <div class="text-3xl mb-2">🌾</div>
            <h4 class="font-bold text-primary text-sm mb-1">Erntedankaltar</h4>
            <p class="text-gray-500 text-xs">Im Oktober</p>
          </div>
          <div class="bg-white p-4 rounded-xl text-center shadow-sm hover:shadow-md transition-shadow">
            <div class="text-3xl mb-2">📿</div>
            <h4 class="font-bold text-primary text-sm mb-1">Oktoberrosenkranz</h4>
            <p class="text-gray-500 text-xs">Im Oktober</p>
          </div>
          <div class="bg-white p-4 rounded-xl text-center shadow-sm hover:shadow-md transition-shadow">
            <div class="text-3xl mb-2">📖</div>
            <h4 class="font-bold text-primary text-sm mb-1">Lektorendienst</h4>
            <p class="text-gray-500 text-xs">Im November</p>
          </div>
          <div class="bg-white p-4 rounded-xl text-center shadow-sm hover:shadow-md transition-shadow">
            <div class="text-3xl mb-2">⛪</div>
            <h4 class="font-bold text-primary text-sm mb-1">Jugendgottesdienst</h4>
            <p class="text-gray-500 text-xs">Regelmäßig</p>
          </div>
        </div>
      </div>
    </section>

    <!-- CTA Section -->
    <section class="py-12 md:py-16 bg-gradient-to-br from-primary to-primary-dark text-white text-center">
      <div class="max-w-4xl mx-auto px-4">
        <h2 class="text-3xl md:text-4xl font-bold mb-4">Du möchtest dabei sein?</h2>
        <p class="text-lg md:text-xl mb-8 text-white/95">
          Komm einfach bei einem unserer Treffen vorbei oder melde dich bei uns!
        </p>
        <router-link 
          to="/kontakt"
          class="inline-block bg-secondary hover:bg-secondary/90 text-gray-900 font-semibold px-8 py-3 rounded-full transition-all transform hover:-translate-y-1 hover:shadow-lg"
        >
          Kontakt aufnehmen
        </router-link>
      </div>
    </section>
  </div>
</template>

<script setup>
// Events page component
</script>
