<script>
  import { testimonials } from "../content";
  // core version + navigation, pagination modules:
  import Swiper from "swiper";
  import { Navigation, Pagination, Autoplay } from "swiper/modules";
  import { onMount } from "svelte";

  import "swiper/css"; // basic Swiper styles
  import "swiper/css/navigation";
  import "swiper/css/pagination";

  // Configure Swiper (install modules)
  Swiper.use([Navigation, Pagination, Autoplay]);

  let swiper;
  onMount(() => {
    swiper = new Swiper(".mySwiper", {
      modules: [Navigation, Pagination, Autoplay], // Optional if you need extra features
      loop: true, // Slides will loop
      slidesPerView: 1, // Number of slides visible at once
      spaceBetween: 30, // Space between slides
      pagination: {
        el: ".swiper-pagination",
        clickable: true,
      },
      autoplay: {
        delay: 5000,
        pauseOnMouseEnter: true,
      },
      // Optional for navigation buttons
      navigation: {
        nextEl: ".swiper-button-next",
        prevEl: ".swiper-button-prev",
      },
    });
  });
</script>

<div class="bg-gray-50 dark:bg-gray-900 py-16">
  <div
    class="container m-auto text-gray-600 dark:text-gray-300 md:px-12 xl:px-6"
  >
    <div class="mb-12 space-y-4 px-6 md:px-0">
      <h2
        class="text-slate-700 text-6xl font-bold leading-[65px] self-center whitespace-nowrap mt-12 max-md:text-4xl max-md:leading-10 max-md:mt-10 text-center"
      >
        Testimonials
      </h2>
      <p class="text-center">
        We don't like to brag, but we don't mind letting our customers do it for
        us. <br />
        Here are a few nice things folks have said about our themes over the years.
      </p>
    </div>
    <div class="swiper mySwiper">
      <div class="swiper-wrapper pb-8">
        {#each testimonials as testimonial}
          <div class="swiper-slide !bg-transparent px-6 md:px-0">
            <div
              class="p-2 border border-gray-100 dark:border-gray-700 rounded-3xl bg-white dark:bg-gray-800 shadow-2xl shadow-gray-600/10 dark:shadow-none md:mx-auto lg:w-10/12 xl:w-8/12"
            >
              <div class="grid md:grid-cols-5">
                <img
                  src="/gallery/bookkeeping3.jpg"
                  class="md:col-span-2 h-full w-full rounded-2xl object-cover"
                  alt=""
                  width="640"
                  height="422"
                  loading="lazy"
                />
                <div
                  class="md:col-span-3 mx-auto space-y-6 p-6 text-center sm:p-8"
                >
                  <div class="mx-auto w-24">
                    <img
                      src="/AR-logo.svg"
                      alt="company logo"
                      height="400"
                      width="142"
                      loading="lazy"
                    />
                  </div>
                  <p>
                    <span class="font-serif">"</span>
                    {testimonial.comment}
                    <span class="font-serif">"</span>
                  </p>
                  <!-- <h6 class="text-lg font-semibold leading-none">John Doe</h6> -->
                </div>
              </div>
            </div>
          </div>
        {/each}
      </div>
      <div class="swiper-pagination" />
    </div>
  </div>
</div>
