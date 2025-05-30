<script setup>
const services = [
  {
    title: 'Tresses',
    description: 'Elegant and protective styles to enhance your natural beauty.',
    image: '/images/services/tresses.png'
  },
  {
    title: 'Braids',
    description: 'Box braids, cornrows, and trendy styles tailored to you.',
    image: '/images/services/braids.jpg'
  },
  {
    title: 'Extensions',
    description: 'Add length and volume with seamless professional extensions.',
    image: '/images/services/extensions.png'
  },
  {
    title: 'Défrisage',
    description: 'Smooth and straighten hair with care for health and shine.',
    image: '/images/services/relaxers.png'
  },
  {
    title: 'Wig Installations',
    description: 'Custom wig fitting and styling for any occasion.',
    image: '/images/services/wig-installations.png'
  },
  {
    title: 'Manicures & Pedicures',
    description: 'Elegant nail care to refresh hands and feet.',
    image: '/images/services/manicure-pedicure.png'
  }
];
</script>

<template>
  <!-- Navbar migliorata -->
  <div class="navbar bg-base-100/50 backdrop-blur-sm fixed top-0 left-0 z-50">
    <div class="flex-none">
      <button class="btn btn-square btn-ghost" aria-label="Menu">
        <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
        </svg>
      </button>
    </div>

    <div class="flex-1">
      <NuxtLink to="https://afrocoiffuremixt.com"
        class="btn btn-ghost text-2xl font-title tracking-wide text-base-content">
        afrocoiffuremixt.com
      </NuxtLink>
    </div>

    <div class="flex-none">
      <label class="swap swap-rotate">
        <input type="checkbox" class="theme-controller" value="light" data-toggle-theme="light,dark" />
        <svg class="swap-off h-10 w-10 fill-current" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
          <path
            d="M5.64,17l-.71.71a1,1,0,0,0,0,1.41,1,1,0,0,0,1.41,0l.71-.71A1,1,0,0,0,5.64,17ZM5,12a1,1,0,0,0-1-1H3a1,1,0,0,0,0,2H4A1,1,0,0,0,5,12Zm7-7a1,1,0,0,0,1-1V3a1,1,0,0,0-2,0V4A1,1,0,0,0,12,5ZM5.64,7.05a1,1,0,0,0,.7.29,1,1,0,0,0,.71-.29,1,1,0,0,0,0-1.41l-.71-.71A1,1,0,0,0,4.93,6.34Zm12,.29a1,1,0,0,0,.7-.29l.71-.71a1,1,0,1,0-1.41-1.41L17,5.64a1,1,0,0,0,0,1.41A1,1,0,0,0,17.66,7.34ZM21,11H20a1,1,0,0,0,0,2h1a1,1,0,0,0,0-2Zm-9,8a1,1,0,0,0-1,1v1a1,1,0,0,0,2,0V20A1,1,0,0,0,12,19ZM18.36,17A1,1,0,0,0,17,18.36l.71.71a1,1,0,0,0,1.41,0,1,1,0,0,0,0-1.41ZM12,6.5A5.5,5.5,0,1,0,17.5,12,5.51,5.51,0,0,0,12,6.5Zm0,9A3.5,3.5,0,1,1,15.5,12,3.5,3.5,0,0,1,12,15.5Z" />
        </svg>
        <svg class="swap-on h-10 w-10 fill-current" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
          <path
            d="M21.64,13a1,1,0,0,0-1.05-.14,8.05,8.05,0,0,1-3.37.73A8.15,8.15,0,0,1,9.08,5.49a8.59,8.59,0,0,1,.25-2A1,1,0,0,0,8,2.36,10.14,10.14,0,1,0,22,14.05,1,1,0,0,0,21.64,13Zm-9.5,6.69A8.14,8.14,0,0,1,7.08,5.22v.27A10.15,10.15,0,0,0,17.22,15.63a9.79,9.79,0,0,0,2.1-.22A8.11,8.11,0,0,1,12.14,19.73Z" />
        </svg>
      </label>
    </div>
  </div>

  <!-- Hero section migliorata -->
  <div class="hero min-h-screen bg-cover bg-center" style="background-image: url('/images/afro-pattern1.png');">
    <div class="hero-overlay bg-base-300/70 backdrop-blur-sm">
    </div>
    <div class="hero-content text-center">
      <div class="max-w-2xl mx-auto space-y-8 px-4">
        <img src="/images/logo.png" alt="Sheila Logo" class="drop-shadow-xl mx-auto w-90 brightness-125" />
        <h1 class="text-5xl md:text-7xl font-title font-bold text-base-content drop-shadow-md">
          Sheila Afro <br />Coiffure Mixt
        </h1>
        <p class="text-2xl md:text-3xl text-secondary font-medium">
          Afro hair & beauty <br> services at your doorstep
        </p>
        <p class="text-lg md:text-xl text-base-content">
          Specializing in tresses, braids, extensions, relaxers, wig installations, and simple manicures & pedicures —
          delivered to your home.
        </p>
        <a href="#services" class="btn btn-primary btn-lg">Book Now</a>
      </div>
    </div>
  </div>

  <!-- Sezione Servizi migliorata -->
  <section id="services" class="relative min-h-screen py-20">
    <!-- Background con blur -->
    <div class="absolute inset-0 z-0">
      <div class="absolute inset-0 bg-cover bg-center" style="background-image: url('/images/afro-pattern.png');">
      </div>
      <div class="absolute inset-0 bg-base-300/70 backdrop-blur-sm"></div>
    </div>

    <!-- Contenuto principale -->
    <div class="container relative z-10 mx-auto px-4">
      <div class="max-w-6xl mx-auto space-y-12">
        <h2 class="text-4xl md:text-5xl font-title text-primary text-center">Our Services</h2>
        <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-8">
          <div v-for="(service, i) in services" :key="i"
            class="card bg-base-200 hover:shadow-xl transition-all duration-300">
            <figure class="relative"> <!-- Rimosso pt-4 -->
              <img :src="service.image" :alt="service.title" class="h-64 w-full object-cover object-top" />
              <!-- Rimosso rounded-t-xl e aumentato h-56 a h-64 -->
            </figure>
            <div class="card-body">
              <h3 class="card-title text-primary">{{ service.title }}</h3>
              <p class="flex-grow text-base-content">{{ service.description }}</p>
              <div class="card-actions justify-end">
                <button class="btn btn-primary btn-sm">
                  Book Now
                  <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 ml-1" fill="none" viewBox="0 0 24 24"
                    stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                      d="M17 8l4 4m0 0l-4 4m4-4H3" />
                  </svg>
                </button>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.font-title {
  font-family: var(--font-title);
}

.text-shadow-lg {
  text-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.transition-all {
  transition-property: all;
  transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);
}
</style>
