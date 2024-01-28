<script>
  import CardService from "../components/Card-Service.svelte";
  const service = [
    {
      heading: "Bookkeeping & Accounting",
      caption: `Financial Accuracy & Transparency for Small & Medium Business`
    },
    {
      heading: "Offshore & Outsourced Services",
      caption: `Reliable partner for Accounting Professional & Firms`
    },
    {
      heading: "Business Consulting",
      caption: `Planning, Business modelling & Growth Strategy`
    },
    {
      heading: "Automated Business Solution",
      caption: `Re-engineering of business with IT & AI`
    },
    {
      heading: "Tailored Business Support",
      caption: `One stop solution for complex businesses`
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
    class="self-center w-full mt-5 px-5 max-md:max-w-full flex flex-col sm:flex-row justify-center"
  >
    <CardService heading={service[0].heading} caption={service[0].caption}/>
    <CardService heading={service[1].heading} caption={service[1].caption}/>
    <CardService heading={service[2].heading} caption={service[2].caption}/>
  </div>
  <div
    class="self-center w-full mt-5 px-5 max-md:max-w-full flex flex-col sm:flex-row justify-center"
  >
    <CardService heading={service[3].heading} caption={service[3].caption}/>
    <CardService heading={service[4].heading} caption={service[4].caption}/>
  </div>
  <div
    class="text-slate-700 text-sm font-bold leading-5 self-center whitespace-nowrap mt-12 max-md:mt-10 text-center scale-150"
  >
    <span class="font-bold">Explore more Services → </span> <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 24 24"><g fill="none" stroke="#000000" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"><path stroke-dasharray="20" stroke-dashoffset="20" d="M21 12H3.5"><animate fill="freeze" attributeName="stroke-dashoffset" dur="0.3s" values="20;0"/></path><path stroke-dasharray="12" stroke-dashoffset="12" d="M3 12L10 19M3 12L10 5"><animate fill="freeze" attributeName="stroke-dashoffset" begin="0.3s" dur="0.2s" values="12;0"/></path></g></svg>
  </div>
</section>
