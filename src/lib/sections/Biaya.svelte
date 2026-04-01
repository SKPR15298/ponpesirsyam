<script>
  const fees = [
    { kebutuhan: 'Syahriyah bulan pertama', biaya: 'Rp 700.000' },
    { kebutuhan: 'Seragam Santri', biaya: 'Rp 1.000.000' },
    { kebutuhan: 'Pendaftaran', biaya: 'Rp 800.000' },
    { kebutuhan: 'Infaq Pembangunan', biaya: 'Rp 500.000' }
  ];

  const totalNumber = fees.reduce((sum, fee) => {
    return sum + parseInt(fee.biaya.replace(/[^0-9]/g, ''), 10);
  }, 0);

  const totalFormatted = `Rp ${totalNumber.toLocaleString('id-ID')}`;
</script>

<div class="aspect-auto w-full px-4 md:px-0 md:max-w-[97dvw] py-4 gap-4 flex flex-col justify-center items-center" id="biaya">
  <div class="w-full flex justify-center items-center font-semibold text-lg md:text-2xl px-4 md:px-0">
    <p class="text-center w-full">Biaya Pendaftaran</p>
  </div>

  <div class="bg-[#1B8048] w-full px-2 py-4 md:p-8 rounded-2xl flex flex-col justify-center overflow-x-auto">
    <table class="w-full text-left text-white border-collapse whitespace-nowrap md:whitespace-normal">
      <thead>
        <tr class="border-b-2 border-white/30 text-md md:text-xl">
          <th class="pb-4 font-semibold px-2">Kebutuhan</th>
          <th class="pb-4 font-semibold text-right px-2">Biaya</th>
        </tr>
      </thead>
      <tbody>
        {#each fees as fee}
          <tr class="border-b border-white/10 last:border-0 hover:bg-white/5 transition-colors">
            <td class="py-4 px-2 text-sm md:text-lg">{fee.kebutuhan}</td>
            <td class="py-4 px-2 text-sm md:text-lg text-right font-medium">{fee.biaya}</td>
          </tr>
        {/each}
      </tbody>
    </table>
  </div>

  <div class="bg-[#1B8048] w-full p-2 md:px-8 md:py-6 rounded-2xl flex flex-col justify-center overflow-x-auto">
    <table class="w-full text-left text-white border-collapse whitespace-nowrap md:whitespace-normal">
      <tbody>
        <tr class="text-sm md:text-xl font-bold">
          <td class="py-2 px-2">Total Keseluruhan</td>
          <td class="py-2 px-2 text-right ">{totalFormatted}</td>
        </tr>
      </tbody>
    </table>
  </div>
</div>