<script setup>

</script>

<template>
    <section class="flex justify-center items-center bg-[url('src/assets/image5.jpg')]  bg-cover bg-center h-[1024px] flex-col w-[1440px] w-full h-screen font-oswald" >
        <div class="border-2 rounded-lg border-white bg-black h-[336px] w-[320px] flex flex-col gap-[24px] p-[24px] ">
            <div class=" ">
                <p class="text-[#F3C17A] ">Nimi</p> 
                <input type="" placeholder="Täisnimi" class="bg-[#2C2C2C]  w-full rounded-lg text-[#F3C17A] p-1 border-2 rounded-lg border-[#F3C17A] pl-2 pt-1 pb-1"/>
            </div>
            <div class=" "> 
                <p class="text-[#F3C17A] f">Email</p>
                <input type="" placeholder="misiganes@gmail.com" class="bg-[#2C2C2C] w-full rounded-lg text-[#F3C17A] p-1 border-2 rounded-lg border-[#F3C17A] pl-2 pt-1 pb-1"/>
            </div>
            <div class=" "> 
                <p class="text-[#F3C17A] ">Telefon</p>
                <input type="" placeholder="+372" class="bg-[#2C2C2C]  w-full rounded-lg text-[#F3C17A] p-1 border-2 rounded-lg  pl-2 pt-1 pb-1 border-[#F3C17A]"/>
            </div>
            <button class="p-1 bg-[#2C2C2C]  text-[#F3C17A] rounded-lg  border-2 w-full">Sisesta</button>
        </div>
        <div class="flex flex-col items-center pt-4 gap-4">
            <h1 class="text-[#F3C17A]  ">Miks ette registreerida?</h1>
            <h2 class="text-[#F3C17A]  ">Meile ette registreeritud kliendid saavad enda esimesel <br> tellimusel tasuta kaasa joogi.</h2>
        </div>
    </section>
</template>
