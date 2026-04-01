<script>
  import image from "$lib/assets/images/3.svg";

  const terms = [
    {
      items: [
        'Berusia minimal 7 tahun (sudah bisa makan & mandi sendiri)',
        'Membawa fotokopi akta kelahiran (1 lembar)',
        'Membawa fotokopi KK (1 lembar)',
        'Pas foto 3x4 (3 lembar)'
      ]
    }
  ];
</script>

<div class="aspect-auto w-full md:max-w-[97dvw] py-4 gap-4 md:gap-8 flex flex-col md:py-10 mt-4" id="syarat">
  <div class="w-full justify-between flex font-semibold text-lg md:text-2xl px-4 md:px-0">
    <p class="md:block hidden">03</p>
    <p class="text-center md:text-right">Syarat & Ketentuan</p>
  </div>

  <div class="flex flex-col md:flex-row gap-4 w-full px-4 md:px-0 items-stretch">
    {#each terms as term, index}
      <div class="bg-[#1B8048] w-full md:w-3/4 p-6 md:p-8 rounded-2xl flex flex-col justify-center">
        <ul class="list-disc list-inside text-white text-left md:text-lg space-y-4">
          {#each term.items as item}
            <li>{item}</li>
          {/each}
        </ul>
      </div>

      {#if index === 0}
        <div class="md:w-1/4 w-full flex-shrink-0 flex">
          <img
            src={image}
            alt="Syarat dan Ketentuan"
            class="w-full h-full min-h-62.5 rounded-2xl object-cover"
          />
        </div>
      {/if}
    {/each}
  </div>
</div>