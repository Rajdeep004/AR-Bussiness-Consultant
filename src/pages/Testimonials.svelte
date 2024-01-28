<script>
  import { testimonials } from "../content";
</script>

<section
  id="testimonials"
  class="bg-neutral-100 self-stretch flex w-full flex-col items-center px-5 py-12 max-md:max-w-full max-md:mt-10"
>
  <div
    class="justify-center text-neutral-600 text-center text-6xl font-bold leading-[72px] tracking-tighter max-w-[555px] mt-3.5 max-md:text-4xl max-md:leading-[54px]"
  >
    Testimonials
  </div>
  <div
    class="slider self-stretch flex flex-col md:flex-row justify-center gap-5 mt-16 mb-52 max-md:max-w-full flex-wrap max-md:justify-center max-md:my-10"
  >
    {#each testimonials as testimonial, index(testimonial.id)}
      <div
        class="item md:w-1/4 opacity-100 hover:scale-105"
        style="padding-left: 28.80px; padding-right: 28.80px; padding-top: 25.20px; padding-bottom: 25.20px; background: white; border-radius: 10.80px; flex-direction: column; justify-content: center; align-items: flex-start; gap: 2rem; display: inline-flex"
  
      >
        <img src="/quote.svg" alt="QuoteImage"/>

        <div
          class="text-2xl"
          style="color: #413D45;  font-weight: 600; word-wrap: break-word"
        >
          { testimonial.comment }
        </div>

        <div
          style="align-self: stretch; padding-bottom: 0.90px; padding-right: 64.14px; flex-direction: column; justify-content: center; align-items: start; display: inline-flex"
        >
          <div
            class="text-md md:text-lg"
            style="color: #006FF2; font-family: Inter; font-weight: 500; word-wrap: break-word"
          >
            { testimonial.author }
          </div>
          <div
            class="text-md md:text-lg"
            style="color: #413D45; font-family: Inter; font-weight: 500; word-wrap: break-word"
          >
            { testimonial.caption }
          </div>
        </div>
      </div>
    {/each}
  </div>
</section>

<style>


</style>
