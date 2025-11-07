<script setup>
import { ref, onMounted, onUnmounted } from 'vue'


const targetDate = new Date('2025-12-24T14:00:00')

const countdown = ref({
  days: 0,
  hours: 0,
  minutes: 0,
  seconds: 0,
})

let interval

const updateCountdown = () => {
  const now = new Date().getTime()
  const distance = targetDate.getTime() - now

  if (distance <= 0) {
    countdown.value = { days: 0, hours: 0, minutes: 0, seconds: 0 }
    clearInterval(interval)
    return
  }

  countdown.value = {
    days: Math.floor(distance / (1000 * 60 * 60 * 24)),
    hours: Math.floor((distance / (1000 * 60 * 60)) % 24),
    minutes: Math.floor((distance / (1000 * 60)) % 60),
    seconds: Math.floor((distance / 1000) % 60),
  }
}

onMounted(() => {
  updateCountdown()
  interval = setInterval(updateCountdown, 1000)
})

onUnmounted(() => clearInterval(interval))
</script>

<template>
<section class="relative h-screen w-full font-oswald font-medium overflow-hidden flex flex-col bg-cover bg-center">
  <div class="absolute inset-0 bg-[url('/src/assets/bg.webp')] bg-cover bg-center blur-sm scale-105"></div>

  <div class="relative flex flex-col items-center justify-center flex-grow text-center px-4">

    <img class="pt-2 w-auto md:w-56 mb-8 h-auto mx-auto" src="/src/assets/logo.png" alt="Primo Burger Logo">

    <h2 class="text-[3rem] sm:text-[5rem] md:text-[8rem] lg:text-[9rem] pt-6 text-orange-500 font-bold drop-shadow-[3px_3px_0px_#000]">
      PEAGI SAABUMAS...
    </h2>

    <h3 class="text-2xl sm:text-3xl md:text-5xl pt-4 text-[#F3C17A] flex flex-col gap-4 items-center">
      VEEBIÄPI AVAME
      <div class="flex gap-4 text-3xl sm:text-4xl md:text-5xl font-semibold">
        <div class="flex flex-col items-center">
          <span>{{ countdown.days }}</span>
          <small class="text-lg md:text-xl font-normal text-orange-500">Päev</small>
        </div>
        <div class="flex flex-col items-center">
          <span>{{ countdown.hours }}</span>
          <small class="text-lg md:text-xl font-normal text-orange-500">Tund</small>
        </div>
        <div class="flex flex-col items-center">
          <span>{{ countdown.minutes }}</span>
          <small class="text-lg md:text-xl font-normal text-orange-500">Minut</small>
        </div>
        <div class="flex flex-col items-center">
          <span>{{ countdown.seconds }}</span>
          <small class="text-lg md:text-xl font-normal text-orange-500">Sekund</small>
        </div>
      </div>
    </h3>
  </div>

  <div class="relative pt-6 flex flex-col items-center justify-end pb-8 gap-4">
    <p class="text-2xl sm:text-3xl md:text-4xl text-orange-500 font-semibold mb-2">
      Skrolli alla!
    </p>
    <img class="w-8 h-8 sm:w-10 sm:h-10 animate-bounce" src="/src/assets/arrow.svg" alt="Arrow Down">
  </div>
</section>
</template>
