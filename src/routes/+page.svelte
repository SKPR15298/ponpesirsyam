<script>
    import Navbar from "$lib/components/Navbar.svelte";
    import Hero from "$lib/sections/Hero.svelte";
    import Profil from "$lib/sections/Profil.svelte";
    import Visi from "$lib/sections/Visi.svelte";
    import Program from "$lib/sections/Program.svelte";
    import Syarat from "$lib/sections/Syarat.svelte";
    import Biaya from "$lib/sections/Biaya.svelte";
    import Confirm from "$lib/sections/Confirm.svelte";
    import Footer from "$lib/components/Footer.svelte";
</script>

<Navbar />

<div class="w-full flex flex-col items-center">
    <Hero />
    <Profil />
    <Visi />
    <Program />
    <Syarat />
    <Biaya />
    <Confirm />
</div>
<Footer />
<style lang="postcss">
    @reference "tailwindcss";
</style>