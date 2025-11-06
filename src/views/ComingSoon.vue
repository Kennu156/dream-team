<script setup>
</script>

<template>
<section class="relative h-screen w-full font-oswald font-medium overflow-hidden flex flex-col bg-cover bg-center">
  <div class="absolute inset-0 bg-[url('src/assets/bg.jpg')] bg-cover bg-center blur-sm scale-105"></div>

  <div class="relative flex flex-col items-center justify-center flex-grow text-center px-4">
    <h1 class="text-4xl md:text-5xl text-orange-500 font-display">Primo Burger</h1>

    <img class="pt-4 w-auto md:w-56 h-auto mx-auto" src="/src/assets/logo.png" alt="Primo Burger Logo">

    <h2 class="text-[3rem] sm:text-[5rem] md:text-[8rem] lg:text-[9rem] pt-6 text-orange-500 font-bold drop-shadow-[3px_3px_0px_#000]">
      PEAGI SAABUMAS...
    </h2>

    <h3 class="text-2xl sm:text-3xl md:text-5xl pt-8 text-[#F3C17A] flex flex-col gap-4">
      VEEBIÄPPI AVAME<span>24.12.2025</span>
    </h3>
  </div>
  <div class="relative flex flex-col items-center justify-end pb-8 mt-auto gap-4">
    <p class="text-2xl sm:text-3xl md:text-4xl text-[#F3C17A] font-semibold mb-2">
      Skrolli alla!
    </p>
    <img class="w-8 h-8 sm:w-10 sm:h-10 animate-bounce" src="/src/assets/arrow.svg" alt="Arrow Down">
  </div>
</section>
</template>
