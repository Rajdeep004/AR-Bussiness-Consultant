<script>
  import { Carousel } from 'flowbite-svelte';
  const images = [
  {
    alt: 'bookkeeping1',
    src: '/gallery/bookkeeping3.jpg',
    title: ''
  },
  {
    alt: 'bookkeeping2',
    src: '/gallery/bookkeeping1.avif',
    title: ''
  },
  {
    alt: 'bookkeeping3',
    src: '/gallery/bookkeeping2.jpg',
    title: ''
  },
];

</script>

<section
  id="hero"
  class="flex flex-col md:flex-row gap-4 container mx-4 mt-16"
>
  <div class="w-full sm:w-1/2 flex flex-col justify-evenly gap-8 lg:gap-0">
    <div>
      <h1 class="text-slate-700 text-6xl font-semibold self-stretch outline-none">
        A & R <br /> Business <br class="sm:hidden"/>  Consultant
      </h1>
      <h2 class="text-zinc-400 text-2xl font-semibold leading-10">
        Your Partner in Financial Growth and Stability!
      </h2>
      <!-- <div
        class="text-slate-700 text-sm font-bold leading-5 self-stretch whitespace-nowrap mt-4 max-md:max-w-full"
      >
        Know more
      </div> -->
    </div>
    <!-- Social Icons -->
    <a href="https://www.linkedin.com/company/a-r-business-consultant-limited" target="_blank" class="inline-flex items-center gap-2 bg-blue-700/85 px-6 py-3 rounded-full text-white font-bold w-max hover:bg-blue-600/85"><svg xmlns="http://www.w3.org/2000/svg" height="28" viewBox="0 0 24 24"><circle cx="4" cy="4" r="2" fill="currentColor" fill-opacity="0"><animate fill="freeze" attributeName="fill-opacity" dur="0.4s" values="0;1"/></circle><g fill="none" stroke="currentColor" stroke-linecap="round" stroke-width="4"><path stroke-dasharray="12" stroke-dashoffset="12" d="M4 10V20"><animate fill="freeze" attributeName="stroke-dashoffset" begin="0.2s" dur="0.2s" values="12;0"/></path><path stroke-dasharray="12" stroke-dashoffset="12" d="M10 10V20"><animate fill="freeze" attributeName="stroke-dashoffset" begin="0.5s" dur="0.2s" values="12;0"/></path><path stroke-dasharray="24" stroke-dashoffset="24" d="M10 15C10 12.2386 12.2386 10 15 10C17.7614 10 20 12.2386 20 15V20"><animate fill="freeze" attributeName="stroke-dashoffset" begin="0.7s" dur="0.5s" values="24;0"/></path></g></svg><span>Linkedin</span></a>
  </div>

  <div class="w-full lg:h-3/4 lg:w-1/2 mb-16">
    <Carousel {images} duration={3000} let:Indicators class="">
      <Indicators 
        activeClass="bg-blue-600/80 px-4" 
        inactiveClass=""
        class="scale-75"
      />
    </Carousel>
  </div>
  
</section>
