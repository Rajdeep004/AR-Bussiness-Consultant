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
  const updateSerIdx = (idx) =>{
    serviceIdx = idx
    console.log("updateSerIdx to:", serviceIdx);
  }
</script>

<Navbar />
<section id="Services" class="container mx-auto flex flex-col md:flex-row">
  <div
    id="sidebar"
    class="md:w-[50%] md:max-h-screen flex flex-col items-center justify-center lg:flex-row"
  >
    <div class="scale-95 space-y-4">
      <SmallService
        idx={0}
        heading={serviceCards[0].heading}
        caption={serviceCards[0].caption}
        on:click={updateSerIdx}
      />
      <SmallService
        idx={1}
        heading={serviceCards[1].heading}
        caption={serviceCards[1].caption}
      />
      <SmallService
        idx={2}
        heading={serviceCards[2].heading}
        caption={serviceCards[2].caption}
        on:click={e => {updateSerIdx(2)}}
    
      />
    </div>
    <div class="scale-95 space-y-4">
      <SmallService
        idx={3}
        heading={serviceCards[3].heading}
        caption={serviceCards[3].caption}
        on:click={e => {updateSerIdx(3)}}
    
      />
      <SmallService
        idx={4}
        heading={serviceCards[4].heading}
        caption={serviceCards[4].caption}
        on:click={e => {updateSerIdx(4)}}
    
      />
    </div>
  </div>
  <MainContent details={services[serviceIdx]} />
</section>
<Footer />
