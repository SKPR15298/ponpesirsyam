<script>
const missions = [
  {
    id: '01',
    title: 'Ahlussunnah Wal Jama’ah',
    desc: 'Mewujudkan generasi hafidz dan hafidzah yang tidak hanya mampu menjaga hafalan, tetapi juga konsisten mengamalkan ajaran Islam yang moderat berlandaskan tradisi dan nilai-nilai luhur Ahlussunnah Wal Jama’ah (ASWAJA) dalam kehidupan bermasyarakat.'
  },
  {
    id: '02',
    title: 'Taqwa & Mutqin',
    desc: 'Membentuk insan bertaqwa dengan kualitas hafalan Al-Qur’an yang kuat dan teruji (mutqin), diiringi dengan pemahaman mendalam terhadap makna ayat untuk diimplementasikan sebagai pedoman hidup komprehensif.'
  },
  {
    id: '03',
    title: 'Kader Bersanad',
    desc: 'Menciptakan kader pengajar Al-Qur’an berdedikasi tinggi dan berkompeten, yang didukung oleh keabsahan hafalan melalui jalur sanad keilmuan yang muttasil (bersambung) hingga ke Rasulullah SAW.'
  }
];
</script>

<div class="aspect-auto w-full md:max-w-[97dvw] mt-4">
  <div class="w-full mx-auto flex-col flex items-center gap-0 md:gap-8  justify-between">
    <h1 class="uppercase text-2xl text-[#FFAF04] w-full sm:max-w-none md:max-w-1/2 text-center font-bold mb-8 md:mb-0">
      “Mencetak generasi qur’ani yang mandiri dan berdedikasi tinggi untuk membumikan Al Qur’an”
    </h1>

    <div class="flex flex-col md:flex-row gap-4 w-full px-4 md:px-0">
      {#each missions as item}
        <div class="bg-[#1B8048] w-full p-6 rounded-2xl flex flex-col gap-4 hover:-translate-y-0.5 hover:shadow-xl transition-all duration-300 hover:cursor-pointer">
          <div class="flex justify-between gap-2">
            <p class="font-bold text-2xl text-white">{item.id}</p>
            <p class="text-2xl text-[#FFAF04] font-semibold">{item.title}</p>
          </div>
          <p class="text-white text-justify md:text-lg">{item.desc}</p>
        </div>
      {/each}
    </div>
  </div>
</div>