<script>
  export const testimonials = [
    {
      id: 1,
      author: "Peter, Belgium",
      caption: "on what he learned when sitting with himself",
      comment:
        "I came to learn that the storyline in my head... was holding me back.",
    },
    {
      id: 2,
      author: "Peter, Belgium",
      caption: "on what he learned when sitting with himself",
      comment:
        "I came to learn that the storyline in my head... was holding me back.",
    },
    {
      id: 3,
      author: "Peter, Belgium",
      caption: "on what he learned when sitting with himself",
      comment:
        "I came to learn that the storyline in my head... was holding me back.",
    },
    {
      id: 4,
      author: "Peter, Belgium",
      caption: "on what he learned when sitting with himself",
      comment:
        "I came to learn that the storyline in my head... was holding me back.",
    },
    {
      id: 5,
      author: "Peter, Belgium",
      caption: "on what he learned when sitting with himself",
      comment:
        "I came to learn that the storyline in my head... was holding me back.",
    },
    {
      id: 6,
      author: "Peter, Belgium",
      caption: "on what he learned when sitting with himself",
      comment:
        "I came to learn that the storyline in my head... was holding me back.",
    },
    {
      id: 7,
      author: "Peter, Belgium",
      caption: "on what he learned when sitting with himself",
      comment:
        "I came to learn that the storyline in my head... was holding me back.",
    },
  ];
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
    class="self-stretch flex items- justify-between gap-5 mt-16 mb-52 px-px max-md:max-w-full max-md:flex-wrap max-md:justify-center max-md:my-10"
  >
    {#each testimonials as testimonial, index(testimonial.id)}
      <div
        style="width: 336.60px; height: 383.40px; padding-left: 28.80px; padding-right: 28.80px; padding-top: 25.20px; padding-bottom: 25.20px; background: white; border-radius: 10.80px; flex-direction: column; justify-content: center; align-items: flex-start; gap: 118.80px; display: inline-flex"
        class="opacity-100 hover:scale-105"
      >
        <img src="/quote.svg" alt="QuoteImage"/>

        <div
          style="width: 254.71pmx; height: 3px; color: #413D45; font-size: 24.30px;  font-weight: 600; line-height: 32.40px; word-wrap: break-word"
        >
          { testimonial.comment }
        </div>

        <div
          style="align-self: stretch; height: 37.80px; padding-bottom: 0.90px; padding-right: 64.14px; flex-direction: column; justify-content: center; align-items: flex-start; gap: 9px; display: inline-flex"
        >
          <div
            style="width: 81.52px; height: 15.30px; color: #006FF2; font-size: 11.70px; font-family: Inter; font-weight: 500; line-height: 16.20px; word-wrap: break-word"
          >
            { testimonial.author }
          </div>
          <div
            style="width: 214.86px; height: 12.60px; color: #413D45; font-size: 9.90px; font-family: Inter; font-weight: 500; line-height: 14.40px; word-wrap: break-word"
          >
            on what he learned when sitting with himself
          </div>
        </div>
      </div>
    {/each}
  </div>
</section>

<style>
</style>
