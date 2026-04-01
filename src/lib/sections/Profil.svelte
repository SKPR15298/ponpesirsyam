    <script>
    import person from "$lib/assets/images/2.svg";
    </script>

    <div
    class="aspect-auto  w-full md:max-w-[97dvw] mt-4"
    id="profil"
    >
        <div class="w-full justify-between flex  font-semibold text-2xl px-4 md:px-0">
            <p class="md:block hidden">01</p>
            <p class="w-full text-center md:text-right">Warisan Sanad yang Terjaga</p>
        </div>
        <div class="w-full mx-auto flex-col  flex items-center gap-0 md:gap-8 py-4 md:py-10 justify-center ">
            <div class="flex flex-col flex-1 gap-4 w-full px-4 md:px-0 ">
                <div class="bg-[#1B8048] p-6 rounded-2xl flex flex-col gap-4">
                <h1 class="underline uppercase text-2xl text-[#FFAF04] font-semibold">
                    Profil
                </h1>

                <p class="text-lg text-white leading-relaxed text-justify md:text-xl">
                    Didirikan pada 7 Juni 2023 oleh Gus Ahmad Alfi, Pondok Tahfidz Gentong
                    menjaga kemurnian bacaan melalui transmisi keilmuan yang jelas.
                    Kami memegang teguh sanad dari KH.R. Munawwir (Krapyak)
                    melalui Gus Mas'udi Fathurrahman.
                </p>
                </div>

                <div class="flex md:flex-row flex-col justify-between gap-4">
                    <div class="bg-[#1B8048] p-6 rounded-2xl w-full">
                        <p class="text-xl font-bold text-white">
                            Sanad Qiraat Sab’ah
                            <span class="font-normal">(7 Imam)</span>
                        </p>
                    </div>

                    <div class="bg-[#1B8048] p-6 rounded-2xl w-full">
                        <p class="text-xl font-bold text-white">
                            Sanad Qiroah Masyhuroh
                            <span class="font-normal">(Imam Ashim)</span>
                        </p>
                    </div>
                </div>
            </div>

            <div class="md:w-1/3 w-full flex-shrink-0  items-center justify-center md:flex">
                <img
                src={person}
                alt="Person"
                class="w-full rounded-2xl object-cover"
                />
            </div>
        </div>
    </div>