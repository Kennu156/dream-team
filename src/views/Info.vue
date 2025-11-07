<script setup>

</script>

<template>
<section class="min-h-screen pb-20 gap-10 flex-col w-full bg-black bg-cover bg-center flex items-center justify-center px-4 py-16">
  
  <div class="max-w-5xl w-full text-center font-oswald bg-black/60 backdrop-blur-md p-8 sm:p-10 md:p-14 rounded-3xl shadow-2xl border border-[#F3C17A]/30">
    <h1 class="mt-2 text-4xl sm:text-5xl md:text-6xl lg:text-7xl font-medium tracking-wide text-[#F3C17A] leading-tight drop-shadow-[2px_2px_4px_#000]">
      KOOSTA BURGER<br />
      ENDA MAITSE JÄRGI!
    </h1>

    <div class="mt-8">
      <img
        src="../assets/burger.gif"
        alt="Koosta enda burger"
        class="mx-auto w-full max-w-lg sm:max-w-xl md:max-w-2xl h-auto rounded-2xl shadow-lg hover:scale-105 transition-transform duration-300 ease-in-out"
      />
    </div>

    <ul class="mt-12 space-y-4 text-xl sm:text-2xl md:text-3xl text-[#F3C17A] leading-snug text-left mx-auto w-fit">
      <li class="list-none flex items-start space-x-3">
        <span class="text-orange-500 text-4xl leading-none">•</span>
        <span>KOMPLEKTEERI ENDA LEMMIK KOMPONENTIDEST</span>
      </li>
      <li class="list-none flex items-start space-x-3">
        <span class="text-orange-500 text-4xl leading-none">•</span>
        <span>SALVESTA LEMMIKUTESSE VÕI TELLI KOHE</span>
      </li>
    </ul>
  </div>
  <h1 class="text-orange-500">REKLAAMVIDEO:</h1>
  <video width="800" controls class="rounded-2xl shadow-lg border border-[#F3C17A]/30">
  <source src="../assets/promtcaramell.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>
</section>

</template>
