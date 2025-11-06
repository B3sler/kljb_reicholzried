<template>
  <div class="w-full">
    <!-- Hero Section -->
    <section class="bg-gradient-to-br from-primary to-primary-dark text-white py-12 md:py-16 text-center">
      <div class="max-w-4xl mx-auto px-4">
        <h1 class="text-4xl md:text-5xl font-bold mb-4">Termine & Veranstaltungen</h1>
        <p class="text-xl text-white/95">Bleib auf dem Laufenden über unsere Events</p>
      </div>
    </section>

    <!-- Calendar Section -->
    <section class="py-12 md:py-16 bg-white">
      <div class="max-w-5xl mx-auto px-4">
        <div class="text-center mb-8">
          <h2 class="text-2xl md:text-3xl font-bold text-primary mb-4">Unsere Veranstaltungen im Überblick</h2>
          <p class="text-gray-600 leading-relaxed max-w-3xl mx-auto">
            Hier findest du alle kommenden Termine und Veranstaltungen der KLJB Reicholzried.
            Von wöchentlichen Treffen bis zu großen Events - sei dabei!
          </p>
        </div>

        <div class="mb-8">
          <div class="relative w-full rounded-xl overflow-hidden shadow-xl bg-white" style="padding-bottom: 75%;">
            <iframe
              src="https://calendar.google.com/calendar/embed?height=600&wkst=2&ctz=Europe%2FBerlin&bgcolor=%23ffffff&showTitle=0&showNav=1&showDate=1&showPrint=0&showTabs=1&showCalendars=0&mode=MONTH"
              class="absolute top-0 left-0 w-full h-full border-0"
              scrolling="no"
              title="KLJB Reicholzried Kalender"
            ></iframe>
          </div>
          <p class="text-center text-gray-500 italic mt-4">
            📅 Tipp: Du kannst den Kalender durchblättern und auf einzelne Termine klicken, um mehr Informationen zu erhalten.
          </p>
        </div>
      </div>
    </section>

    <!-- Regular Events -->
    <section class="py-12 md:py-16 bg-gray-50">
      <div class="max-w-7xl mx-auto px-4">
        <h2 class="text-2xl md:text-3xl font-bold text-center text-primary mb-10">Regelmäßige Aktivitäten</h2>
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6">
          <div class="bg-white p-6 rounded-xl shadow-md hover:shadow-xl transition-all transform hover:-translate-y-1 text-center">
            <div class="text-5xl mb-3">📅</div>
            <h3 class="text-lg font-bold text-primary mb-2">Wöchentliche Treffen</h3>
            <p class="text-gray-600 text-sm leading-relaxed">Mindestens einmal pro Woche treffen wir uns zu Aktivitäten, Spieleabenden und Event-Planung.</p>
          </div>

          <div class="bg-white p-6 rounded-xl shadow-md hover:shadow-xl transition-all transform hover:-translate-y-1 text-center">
            <div class="text-5xl mb-3">🎅</div>
            <h3 class="text-lg font-bold text-primary mb-2">Nikolausbesuche</h3>
            <p class="text-gray-600 text-sm leading-relaxed">Am 6. Dezember besuchen wir als KLJB die Familien und bringen den Nikolaus zu den Kindern.</p>
          </div>

          <div class="bg-white p-6 rounded-xl shadow-md hover:shadow-xl transition-all transform hover:-translate-y-1 text-center">
            <div class="text-5xl mb-3">🎄</div>
            <h3 class="text-lg font-bold text-primary mb-2">Adventssingen</h3>
            <p class="text-gray-600 text-sm leading-relaxed">Wir nehmen am Adventssingen teil, organisiert vom Pfarrgemeinderat in der Pfarrkirche.</p>
          </div>

          <div class="bg-white p-6 rounded-xl shadow-md hover:shadow-xl transition-all transform hover:-translate-y-1 text-center">
            <div class="text-5xl mb-3">🎵</div>
            <h3 class="text-lg font-bold text-primary mb-2">Seniorensingen</h3>
            <p class="text-gray-600 text-sm leading-relaxed">Beim Seniorensingen sammeln wir für einen guten Zweck und bringen Freude zu den Senioren.</p>
          </div>
        </div>
      </div>
    </section>

    <!-- Annual Highlights -->
    <section class="py-12 md:py-16 bg-white">
      <div class="max-w-5xl mx-auto px-4">
        <h2 class="text-2xl md:text-3xl font-bold text-center text-primary mb-10">Jahreshighlights</h2>
        <div class="space-y-6">
          <div class="flex flex-col md:flex-row gap-4 items-start">
            <div class="flex-shrink-0 w-full md:w-32 text-center md:text-right">
              <span class="inline-block bg-gradient-to-br from-primary to-primary-dark text-white px-4 py-2 rounded-xl font-bold shadow-md">Januar</span>
            </div>
            <div class="flex-1 bg-gray-50 p-6 rounded-xl border-l-4 border-secondary">
              <h3 class="text-xl font-bold text-primary mb-2">🎉 PARTY #1</h3>
              <p class="font-semibold text-gray-700 mb-2">Reithalle Dietmannsried</p>
              <p class="text-gray-600 leading-relaxed">Die erste große Party des Jahres im Allgäu! Mit hochkarätigen DJs und Acts feiern wir den Start ins neue Jahr. 2025 feierten wir unser zehnjähriges Jubiläum!</p>
            </div>
          </div>

          <div class="flex flex-col md:flex-row gap-4 items-start">
            <div class="flex-shrink-0 w-full md:w-32 text-center md:text-right">
              <span class="inline-block bg-gradient-to-br from-primary to-primary-dark text-white px-4 py-2 rounded-xl font-bold shadow-md">Februar</span>
            </div>
            <div class="flex-1 bg-gray-50 p-6 rounded-xl border-l-4 border-secondary">
              <h3 class="text-xl font-bold text-primary mb-2">🍺 Bockbierfest</h3>
              <p class="font-semibold text-gray-700 mb-2">Jugendheim Reicholzried</p>
              <p class="text-gray-600 leading-relaxed">Seit Anfang der 80er Jahre organisieren wir unser zünftiges Bockbierfest mit Musik, Weißwurst und Bier.</p>
            </div>
          </div>

          <div class="flex flex-col md:flex-row gap-4 items-start">
            <div class="flex-shrink-0 w-full md:w-32 text-center md:text-right">
              <span class="inline-block bg-gradient-to-br from-primary to-primary-dark text-white px-4 py-2 rounded-xl font-bold shadow-md">Mai</span>
            </div>
            <div class="flex-1 bg-gray-50 p-6 rounded-xl border-l-4 border-secondary">
              <h3 class="text-xl font-bold text-primary mb-2">🌳 Maibaum aufstellen</h3>
              <p class="font-semibold text-gray-700 mb-2">Vor dem Gasthaus "Rößle"</p>
              <p class="text-gray-600 leading-relaxed">Traditionell am 1. Mai ab 13:00 Uhr. Mit anschließendem Maifest (Kaffee und Kuchen) und musikalischer Umrahmung durch die Musikkapelle Reicholzried.</p>
            </div>
          </div>

          <div class="flex flex-col md:flex-row gap-4 items-start">
            <div class="flex-shrink-0 w-full md:w-32 text-center md:text-right">
              <span class="inline-block bg-gradient-to-br from-primary to-primary-dark text-white px-4 py-2 rounded-xl font-bold shadow-md">Juni</span>
            </div>
            <div class="flex-1 bg-gray-50 p-6 rounded-xl border-l-4 border-secondary">
              <h3 class="text-xl font-bold text-primary mb-2">☀️ Sonnwendfeuer</h3>
              <p class="font-semibold text-gray-700 mb-2">Unterhalb der Kirche</p>
              <p class="text-gray-600 leading-relaxed">Am 21. Juni findet das traditionelle Sonnwendfeuer statt, mit anschließender Open-Air-Party ab 21:00 Uhr.</p>
            </div>
          </div>

          <div class="flex flex-col md:flex-row gap-4 items-start">
            <div class="flex-shrink-0 w-full md:w-32 text-center md:text-right">
              <span class="inline-block bg-gradient-to-br from-primary to-primary-dark text-white px-4 py-2 rounded-xl font-bold shadow-md">Oktober</span>
            </div>
            <div class="flex-1 bg-gray-50 p-6 rounded-xl border-l-4 border-secondary">
              <h3 class="text-xl font-bold text-primary mb-2">🍷 Weinfest</h3>
              <p class="font-semibold text-gray-700 mb-2">Jugendheim Reicholzried</p>
              <p class="text-gray-600 leading-relaxed">Im Herbst laden wir zum gemütlichen Weinfest ein. Ab 20:00 Uhr verschiedene Weine mit herbstlichen Schmankerln. Ab 22:00 Uhr Barbetrieb und Partynacht. Einlass ab 16 Jahren.</p>
            </div>
          </div>

          <div class="flex flex-col md:flex-row gap-4 items-start">
            <div class="flex-shrink-0 w-full md:w-32 text-center md:text-right">
              <span class="inline-block bg-gradient-to-br from-primary to-primary-dark text-white px-4 py-2 rounded-xl font-bold shadow-md">Sommer</span>
            </div>
            <div class="flex-1 bg-gray-50 p-6 rounded-xl border-l-4 border-secondary">
              <h3 class="text-xl font-bold text-primary mb-2">🚐 Landjugendausflug</h3>
              <p class="font-semibold text-gray-700 mb-2">Wechselnde Ziele</p>
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
