<script>
  const programs = [
    {
      title: 'Pendidikan Formal',
      items: [
        'Raudhatul Athfal (RA / TK)',
        'Madrasah Ibtidaiyah (MI)',
        'Madrasah Tsanawiyah (MTs)',
        'Sekolah Menengah Kejuruan (SMK)'
      ]
    },
    {
      title: 'Pendidikan Pesantren',
      items: [
        'Tahsin Al-Qur’an',
        'Tahfidz Al-Qur’an',
        "Belajar Qiraat Sab'ah (cara membaca al-qur'an versi 7 Imam)"
      ]
    }
  ];
</script>

<div class="aspect-auto w-full md:max-w-[97dvw] py-4 gap-4 md:gap-8 flex flex-col md:py-10 mt-4"
  id="program">
  <div class="w-full justify-between flex font-semibold text-lg md:text-2xl px-4 md:px-0">
    <p class="text-center md:text-right">Program Pendidikan</p>
    <p class="md:block hidden">02</p>
  </div>

  <div class="flex flex-col md:flex-row gap-4 w-full px-4 md:px-0">
    {#each programs as program}
      <div class="bg-[#1B8048] w-full p-6 rounded-2xl flex flex-col gap-4 hover:-translate-y-0.5 hover:shadow-xl transition-all duration-300 hover:cursor-pointer">
        <p class="font-bold text-base md:text-2xl text-white w-full text-center">{program.title}</p>
        <ul class="list-disc list-inside text-white text-justify text-md md:text-lg">
          {#each program.items as item}
            <li>{item}</li>
          {/each}
        </ul>
      </div>
    {/each}
  </div>
</div>