<script>
  import Navbar from "./Navbar.svelte";
  import Footer from "./Footer.svelte";
  import ServiceCard from "../components/Small-service.svelte";
  import MainContent from "../components/Main-Content.svelte";
  import { services } from "../content";
  import SmallService from "../components/Small-service.svelte";

  const serviceCards = [
    {
      heading: "Bookkeeping & Accounting",
      caption: `Financial Accuracy & Transparency for Small & Medium Business`,
    },
    {
      heading: "Offshore & Outsourced Services",
      caption: `Reliable partner for Accounting Professional & Firms`,
    },
    {
      heading: "Business Consulting",
      caption: `Planning, Business modelling & Growth Strategy`,
    },
    {
      heading: "Automated Business Solution",
      caption: `Re-engineering of business with IT & AI`,
    },
    {
      heading: "Tailored Business Support",
      caption: `One stop solution for complex businesses`,
    },
  ];

  let serviceIdx = -1; // Stores the currently selected service name
  const updateSerIdx = (e) =>{
    serviceIdx = e.detail
    console.log("updateSerIdx to:", serviceIdx );
  }
</script>

<Navbar />
<section id="Services" class="container mx-auto flex flex-col md:flex-row md:max-h-screen gap-12">
  <div
    id="sidebar"
    class="md:w-1/2 md:max-h-screen lg:flex flex-col items-center justify-center lg:flex-row"
  > 
    <div class="hidden scale-95 space-y-4 gap-4 lg:block">
      <SmallService
        idx={0}
        heading={serviceCards[0].heading}
        caption={serviceCards[0].caption}
        isSelected={serviceIdx == 0}
        on:addIdx={updateSerIdx}
      />
      <SmallService
        idx={1}
        heading={serviceCards[1].heading}
        caption={serviceCards[1].caption}
        isSelected={serviceIdx == 1}
        on:addIdx={updateSerIdx}
      />
      <SmallService
        idx={2}
        heading={serviceCards[2].heading}
        caption={serviceCards[2].caption}
        isSelected={serviceIdx == 2}
        on:addIdx={updateSerIdx}
      />
    </div>
    <div class="hidden scale-95 space-y-4 gap-4 lg:block">
      <SmallService
        idx={3}
        heading={serviceCards[3].heading}
        caption={serviceCards[3].caption}
        isSelected={serviceIdx == 3}
        on:addIdx={updateSerIdx}
      />
      <SmallService
        idx={4}
        heading={serviceCards[4].heading}
        caption={serviceCards[4].caption}
        isSelected={serviceIdx == 4}
        on:addIdx={updateSerIdx}
      />
    </div>
    <div class="lg:hidden flex gap-4 overflow-x-auto overscroll-none no-scrollbar py-8">
      {#each serviceCards as card,index }
        <SmallService 
          idx={index}
          heading={card.heading}
          caption={card.caption}
          isSelected={serviceIdx == index}
          on:addIdx={updateSerIdx}
        />
      {/each}
    </div>
  </div>
  <MainContent details={services[serviceIdx]} />
</section>
<Footer />

<style>
  /* Hide scrollbar for Chrome, Safari and Opera */
  .no-scrollbar::-webkit-scrollbar {
    display: none;
  }
  /* Hide scrollbar for IE, Edge and Firefox */
  .no-scrollbar {
    -ms-overflow-style: none;  /* IE and Edge */
    scrollbar-width: none;  /* Firefox */
  }
</style>