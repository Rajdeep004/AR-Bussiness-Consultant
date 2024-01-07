<script>
  import CardService from "../components/Card-Service.svelte";
</script>

<section class="container mx-auto my-4">
  <div
    class="text-slate-700 text-6xl font-bold leading-[65px] self-center whitespace-nowrap mt-32 max-md:text-4xl max-md:leading-10 max-md:mt-10 text-center"
  >
    Services
  </div>
  <div
    class="self-center w-full max-w-[1320px] mt-5 px-5 max-md:max-w-full flex flex-col sm:flex-row"
  >
    <CardService />
    <CardService />
    <CardService />
    <CardService />
  </div>
  <div
    class="self-center w-full max-w-[1320px] mt-5 px-5 max-md:max-w-full flex flex-col sm:flex-row"
  >
    <CardService />
    <CardService />
    <CardService />
    <CardService />
  </div>
  <div
    class="text-slate-700 text-sm font-bold leading-5 self-center whitespace-nowrap mt-12 max-md:mt-10 text-center"
  >
    <span class="font-bold">Explore more Services</span>
    <span class=""> → </span>
  </div>
</section>
