<script>
  import Navbar from "./Navbar.svelte";
  import Footer from "./Footer.svelte";
  import ServiceCard from "../components/Small-service.svelte";
  import { services } from "../content";

  const serviceCards = [
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

<Navbar />
<section id="Services" class="container mx-auto">
  <div class="w-full">
    {#each services as service,index}
      <div
        class={`
            flex flex-col md:flex-row items-center justify-evenl m-8 gap-4 ${index%2 ? "md:flex-row-reverse" : "md:flex-row"}
        `}
      >
        <ServiceCard 
            heading={serviceCards[index].heading} 
            caption={serviceCards[index].caption} 
        />
        <article class="text-justify">
          <h1 class="text-4xl font-bold">{service.title}</h1>
          <p>{service.description}</p>
          <div class=" flex-col md:flex-row gap-8">
            <div class="md:w-1/3">
              <h2 class="text-2xl font-semibold">Our Offerings</h2>
              <ul>
                {#each service.offerings as offer}
                  <li>{offer}</li>
                {/each}
              </ul>
            </div>
            <div class="md:w-2/3">
              <h2 class="text-2xl font-semibold">
                Why to choose {service.title} ?
              </h2>
              <ul>
                {#each service.whyChoose as str}
                  <li>{str}</li>
                {/each}
              </ul>
            </div>
          </div>
        </article>
      </div>
    {/each}
  </div>
</section>
<Footer />
