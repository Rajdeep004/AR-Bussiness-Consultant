<script>
  import CardService from "../components/Card-Service.svelte";
  const service = [
    {
      heading: "Bookkeeping",
      caption: ``
    },
    {
      heading: "Accounting",
      caption: ``
    },
    {
      heading: "Offshore",
      caption: ``
    },
    {
      heading: "Outsourced Services",
      caption: ``
    },
    {
      heading: "Business Consulting",
      caption: `Planning, Business Modeling & Growth Strategy`
    },
    
  ]
</script>

<section class="container mx-auto my-4">
  <div
    class="text-slate-700 text-6xl font-bold leading-[65px] self-center whitespace-nowrap mt-32 max-md:text-4xl max-md:leading-10 max-md:mt-10 text-center"
  >
    Services
  </div>
  <div
    class="self-center w-full max-w-[1320px] mt-5 px-5 max-md:max-w-full flex flex-col sm:flex-row justify-center"
  >
    <CardService heading={service[0].heading} caption=""/>
    <CardService heading={service[1].heading} caption=""/>
    <CardService heading={service[2].heading} caption=""/>
  </div>
  <div
    class="self-center w-full max-w-[1320px] mt-5 px-5 max-md:max-w-full flex flex-col sm:flex-row justify-center"
  >
    <CardService heading={service[3].heading} caption=""/>
    <CardService heading={service[4].heading} caption=""/>
  </div>
  <div
    class="text-slate-700 text-sm font-bold leading-5 self-center whitespace-nowrap mt-12 max-md:mt-10 text-center"
  >
    <span class="font-bold">Explore more Services</span>
    <span class=""> → </span>
  </div>
</section>
