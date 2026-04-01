<script>
  import logo from "$lib/assets/images/logoirsyadul.svg";
</script>

<nav class="navbar sticky top-0 z-10 shadow-base-300/20 shadow-sm md:flex-row bg-base-100">

  <div class="navbar-start w-full justify-between flex items-center ">

    <a class="text-base-content text-xl font-bold no-underline flex items-center" href="/">
      <img src={logo} alt="Logo" class="inline-block w-8 md:w-12 mr-2" />
      <p class="hidden md:block">PPTQ Irsyadul Mubtadi'in</p>
    </a>

    <ul class="menu w-full hidden md-block md:w-auto flex-col md:flex-row md:menu-horizontal gap-1 md:gap-2 p-4 md:p-0 text-base font-semibold">
      <li><a href="#profil" class="hover:text-[#1B8048] hover:underline">Profil</a></li>
      <li><a href="#program" class="hover:text-[#1B8048] hover:underline">Program</a></li>
      <li><a href="#biaya" class="hover:text-[#1B8048] hover:underline">Biaya</a></li>
      <li><button class="rounded-lg px-4 py-2 transform transition-all duration-300 bg-[#1B8048] hover:bg-transparent hover:ring-2 hover:ring-[#1B8048] text-white hover:text-[#1B8048]">Daftar Sekarang</button></li>
    </ul>

    <div class="md:hidden ml-auto">
      <button
        aria-label="Burger menu toggle"
        type="button"
        class="collapse-toggle btn-text btn-secondary btn-sm"
        data-collapse="#navbar-collapse"
      >
        <span class="icon-[tabler--menu-2] size-5"></span>
      </button>
    </div>

  </div>

  <div
    id="navbar-collapse"
    class="collapse hidden absolute top-full left-0 w-full bg-base-100 shadow-lg rounded-b-box z-50
           md:static md:shadow-none md:w-auto"
  >
    <ul class="menu w-full md:w-auto flex-col md:flex-row md:menu-horizontal gap-1 md:gap-2 p-4 md:p-0 text-base">
      <li><a href="#profil">Profil</a></li>
      <li><a href="#program">Program</a></li>
      <li><a href="#biaya">Biaya</a></li>
    </ul>
  </div>

</nav>