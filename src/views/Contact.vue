<script setup>

</script>

<template>
<section class="flex flex-col items-center justify-center min-h-screen w-full bg-[url('src/assets/image5.jpg')] bg-cover bg-center font-oswald px-4 py-12">
  <div class="bg-black/70 backdrop-blur-md border border-[#F3C17A]/40 rounded-2xl shadow-[0_0_25px_rgba(243,193,122,0.2)] p-6 sm:p-8 md:p-10 w-full max-w-md flex flex-col gap-6 text-[#F3C17A]">
    <h2 class="text-center text-2xl sm:text-3xl font-semibold mb-2">Registreeru ette</h2>

    <div class="flex flex-col gap-2">
      <label for="name" class="text-[#F3C17A]/90">Nimi</label>
      <input
        id="name"
        type="text"
        placeholder="Täisnimi"
        class="bg-[#2C2C2C]/80 text-[#F3C17A] placeholder-[#F3C17A]/50 rounded-lg p-2 border border-[#F3C17A]/50 focus:border-[#F3C17A] focus:ring-2 focus:ring-[#F3C17A]/40 outline-none transition-all duration-300"
      />
    </div>

    <div class="flex flex-col gap-2">
      <label for="email" class="text-[#F3C17A]/90">Email</label>
      <input
        id="email"
        type="email"
        placeholder="misiganes@gmail.com"
        class="bg-[#2C2C2C]/80 text-[#F3C17A] placeholder-[#F3C17A]/50 rounded-lg p-2 border border-[#F3C17A]/50 focus:border-[#F3C17A] focus:ring-2 focus:ring-[#F3C17A]/40 outline-none transition-all duration-300"
      />
    </div>

    <div class="flex flex-col gap-2">
      <label for="phone" class="text-[#F3C17A]/90">Telefon</label>
      <input
        id="phone"
        type="tel"
        placeholder="+372"
        class="bg-[#2C2C2C]/80 text-[#F3C17A] placeholder-[#F3C17A]/50 rounded-lg p-2 border border-[#F3C17A]/50 focus:border-[#F3C17A] focus:ring-2 focus:ring-[#F3C17A]/40 outline-none transition-all duration-300"
      />
    </div>

    <button
      class="mt-2 bg-gradient-to-r from-[#F3C17A] to-orange-500 text-black font-semibold rounded-lg py-2 transition-transform duration-300 hover:cursor-pointer hover:scale-105 hover:shadow-[0_0_20px_rgba(243,193,122,0.4)]"
    >
      Sisesta
    </button>
  </div>

  <div class="flex flex-col items-center text-center pt-12 px-4 max-w-2xl">
    <h1 class="text-2xl sm:text-3xl text-[#F3C17A] font-semibold mb-4">
      Miks ette registreerida?
    </h1>
    <h2 class="text-lg sm:text-xl text-[#F3C17A]/90 leading-relaxed">
      Meile ette registreeritud kliendid saavad enda esimesel tellimusel
      <span class="text-orange-400 font-semibold">tasuta kaasa joogi.</span>
    </h2>
  </div>
</section>

</template>
