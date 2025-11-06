<template>
  <div class="w-full">
    <!-- Hero Section -->
    <section class="bg-gradient-to-br from-primary to-primary-dark text-white py-12 md:py-16 text-center">
      <div class="max-w-4xl mx-auto px-4">
        <h1 class="text-4xl md:text-5xl font-bold mb-4">Kontakt</h1>
        <p class="text-xl text-white/95">Wir freuen uns auf deine Nachricht!</p>
      </div>
    </section>

    <!-- Contact Content -->
    <section class="py-12 md:py-16 bg-gray-50">
      <div class="max-w-7xl mx-auto px-4">
        <div class="grid grid-cols-1 lg:grid-cols-5 gap-8">
          <!-- Contact Information -->
          <div class="lg:col-span-2">
            <div class="bg-white p-6 md:p-8 rounded-xl shadow-lg sticky top-20">
              <h2 class="text-2xl font-bold text-primary mb-6">Kontaktinformationen</h2>
              
              <div class="space-y-6">
                <div class="flex items-start gap-4">
                  <div class="text-3xl flex-shrink-0">📍</div>
                  <div>
                    <h3 class="font-bold text-primary mb-1">Adresse</h3>
                    <p class="text-gray-600">Im Winkel 24</p>
                    <p class="text-gray-600">87463 Reicholzried</p>
                  </div>
                </div>

                <div class="flex items-start gap-4">
                  <div class="text-3xl flex-shrink-0">📧</div>
                  <div>
                    <h3 class="font-bold text-primary mb-1">E-Mail</h3>
                    <a href="mailto:kljbreicholzried@t-online.de" class="text-primary hover:text-secondary transition-colors">
                      kljbreicholzried@t-online.de
                    </a>
                  </div>
                </div>

                <div class="flex items-start gap-4">
                  <div class="text-3xl flex-shrink-0">📞</div>
                  <div>
                    <h3 class="font-bold text-primary mb-1">Telefon</h3>
                    <a href="tel:+4983741354" class="text-primary hover:text-secondary transition-colors">
                      08374 / 1354
                    </a>
                  </div>
                </div>

                <div class="flex items-start gap-4">
                  <div class="text-3xl flex-shrink-0">👤</div>
                  <div>
                    <h3 class="font-bold text-primary mb-1">Vorstand</h3>
                    <p class="text-gray-600 font-semibold">Jonas Besler</p>
                  </div>
                </div>
              </div>

              <!-- Social Media -->
              <div class="mt-8 pt-8 border-t border-gray-200">
                <h3 class="font-bold text-primary mb-4">Folge uns auf Social Media</h3>
                <div class="space-y-3">
                  <a 
                    href="https://www.instagram.com/kljb_reicholzried/" 
                    target="_blank" 
                    rel="noopener noreferrer" 
                    class="flex items-center gap-3 p-3 bg-gray-50 rounded-lg hover:bg-primary hover:text-white transition-all group"
                  >
                    <span class="text-2xl">📷</span>
                    <span class="font-medium">@kljb_reicholzried</span>
                  </a>
                  <a 
                    href="https://www.facebook.com/KLJBReicholzried" 
                    target="_blank" 
                    rel="noopener noreferrer" 
                    class="flex items-center gap-3 p-3 bg-gray-50 rounded-lg hover:bg-primary hover:text-white transition-all group"
                  >
                    <span class="text-2xl">📘</span>
                    <span class="font-medium">KLJB Reicholzried</span>
                  </a>
                </div>
              </div>

              <!-- Youth Home Info -->
              <div class="mt-6 p-4 bg-gradient-to-br from-gray-50 to-gray-100 rounded-lg border-l-4 border-secondary">
                <h3 class="font-bold text-primary mb-2">Jugendheim Reicholzried</h3>
                <p class="text-gray-700 font-semibold">Bildhauerweg 3</p>
                <p class="text-gray-700">87463 Reicholzried</p>
                <p class="text-gray-600 text-sm italic mt-2">
                  Unser Jugendheim ist der zentrale Treffpunkt für alle Aktivitäten.
                </p>
              </div>
            </div>
          </div>

          <!-- Contact Form -->
          <div class="lg:col-span-3">
            <div class="bg-white p-6 md:p-8 rounded-xl shadow-lg">
              <h2 class="text-2xl font-bold text-primary mb-6">Schreib uns eine Nachricht</h2>
              <form @submit.prevent="handleSubmit" class="space-y-5">
                <div>
                  <label for="name" class="block text-gray-700 font-semibold mb-2">Name *</label>
                  <input
                    type="text"
                    id="name"
                    v-model="formData.name"
                    required
                    placeholder="Dein Name"
                    class="w-full px-4 py-3 border-2 border-gray-200 rounded-lg focus:border-primary focus:outline-none transition-colors"
                  />
                </div>

                <div>
                  <label for="email" class="block text-gray-700 font-semibold mb-2">E-Mail *</label>
                  <input
                    type="email"
                    id="email"
                    v-model="formData.email"
                    required
                    placeholder="deine.email@beispiel.de"
                    class="w-full px-4 py-3 border-2 border-gray-200 rounded-lg focus:border-primary focus:outline-none transition-colors"
                  />
                </div>

                <div>
                  <label for="phone" class="block text-gray-700 font-semibold mb-2">Telefon (optional)</label>
                  <input
                    type="tel"
                    id="phone"
                    v-model="formData.phone"
                    placeholder="Deine Telefonnummer"
                    class="w-full px-4 py-3 border-2 border-gray-200 rounded-lg focus:border-primary focus:outline-none transition-colors"
                  />
                </div>

                <div>
                  <label for="subject" class="block text-gray-700 font-semibold mb-2">Betreff *</label>
                  <input
                    type="text"
                    id="subject"
                    v-model="formData.subject"
                    required
                    placeholder="Worum geht es?"
                    class="w-full px-4 py-3 border-2 border-gray-200 rounded-lg focus:border-primary focus:outline-none transition-colors"
                  />
                </div>

                <div>
                  <label for="message" class="block text-gray-700 font-semibold mb-2">Nachricht *</label>
                  <textarea
                    id="message"
                    v-model="formData.message"
                    required
                    rows="6"
                    placeholder="Deine Nachricht an uns..."
                    class="w-full px-4 py-3 border-2 border-gray-200 rounded-lg focus:border-primary focus:outline-none transition-colors resize-none"
                  ></textarea>
                </div>

                <button 
                  type="submit" 
                  :disabled="isSubmitting"
                  class="w-full bg-primary hover:bg-primary-dark text-white font-semibold px-8 py-4 rounded-full transition-all transform hover:-translate-y-1 hover:shadow-lg disabled:opacity-70 disabled:cursor-not-allowed disabled:transform-none"
                >
                  {{ isSubmitting ? 'Wird gesendet...' : 'Nachricht senden' }}
                </button>

                <div v-if="submitMessage" class="p-4 rounded-lg" :class="submitMessageType === 'success' ? 'bg-green-100 text-green-800 border border-green-200' : 'bg-red-100 text-red-800 border border-red-200'">
                  {{ submitMessage }}
                </div>

                <p class="text-gray-500 text-sm">
                  * Pflichtfelder<br>
                  <span class="text-xs">Hinweis: Dies ist ein Demo-Formular. Die eingegebenen Daten werden nicht tatsächlich versendet.</span>
                </p>
              </form>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Join Section -->
    <section class="py-12 md:py-16 bg-white">
      <div class="max-w-6xl mx-auto px-4 text-center">
        <h2 class="text-2xl md:text-3xl font-bold text-primary mb-4">Werde Teil unserer Gemeinschaft!</h2>
        <p class="text-gray-600 leading-relaxed max-w-3xl mx-auto mb-10">
          Junge Menschen zwischen 14 und 27 Jahren sind herzlich willkommen,
          bei uns mitzumachen. Komm einfach bei einem unserer wöchentlichen Treffen vorbei
          oder kontaktiere uns für mehr Informationen.
        </p>
        <div class="grid grid-cols-2 md:grid-cols-4 gap-6 max-w-4xl mx-auto">
          <div class="flex flex-col items-center gap-2">
            <div class="text-5xl">🤝</div>
            <span class="text-primary font-semibold">Neue Freunde finden</span>
          </div>
          <div class="flex flex-col items-center gap-2">
            <div class="text-5xl">🎉</div>
            <span class="text-primary font-semibold">Tolle Events erleben</span>
          </div>
          <div class="flex flex-col items-center gap-2">
            <div class="text-5xl">💪</div>
            <span class="text-primary font-semibold">Verantwortung übernehmen</span>
          </div>
          <div class="flex flex-col items-center gap-2">
            <div class="text-5xl">🌱</div>
            <span class="text-primary font-semibold">Dorf mitgestalten</span>
          </div>
        </div>
      </div>
    </section>

    <!-- Organization Section -->
    <section class="py-12 md:py-16 bg-gradient-to-br from-primary to-primary-dark text-white text-center">
      <div class="max-w-4xl mx-auto px-4">
        <h2 class="text-2xl md:text-3xl font-bold mb-4">Teil einer größeren Bewegung</h2>
        <p class="text-lg leading-relaxed mb-8 text-white/95 max-w-3xl mx-auto">
          Die KLJB Reicholzried ist Teil des KLJB Kreisverbandes Kempten im Diözesanverband Augsburg
          und gehört zur bundesweiten Katholischen Landjugendbewegung.
        </p>
        <div class="flex flex-col md:flex-row justify-center gap-4 max-w-2xl mx-auto">
          <a 
            href="https://www.kljb-bayern.de" 
            target="_blank" 
            rel="noopener noreferrer" 
            class="bg-white/10 hover:bg-secondary hover:text-gray-900 text-white px-6 py-3 rounded-full font-semibold border-2 border-white/30 hover:border-secondary transition-all transform hover:-translate-y-1"
          >
            KLJB Bayern
          </a>
          <a 
            href="https://kljb-augsburg.de" 
            target="_blank" 
            rel="noopener noreferrer" 
            class="bg-white/10 hover:bg-secondary hover:text-gray-900 text-white px-6 py-3 rounded-full font-semibold border-2 border-white/30 hover:border-secondary transition-all transform hover:-translate-y-1"
          >
            KLJB Diözesanverband Augsburg
          </a>
          <a 
            href="https://www.kljb.org" 
            target="_blank" 
            rel="noopener noreferrer" 
            class="bg-white/10 hover:bg-secondary hover:text-gray-900 text-white px-6 py-3 rounded-full font-semibold border-2 border-white/30 hover:border-secondary transition-all transform hover:-translate-y-1"
          >
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
