<script>
  export let details;
</script>

{#if details}
  <section class="md:w-1/2 2xl:w-[60%]">
    <h1 class="text-3xl font-bold">{details.title}</h1>
    <p>{details.description}</p>
    <h3 class="text-xl font-bold">Our Offerings</h3>
    <ul>
      {#each details.offerings as offer}
        <li>{offer}</li>
      {/each}
    </ul>
    <h3 class="text-xl font-bold">{details.question}</h3>
    <ul>
      {#each details.whyChoose as str}
        <li>{str}</li>
      {/each}
    </ul>
  </section>
{:else}
  <div class="flex flex-col justify-evenly">
    <div>
      <div class="text-slate-700 text-6xl font-semibold self-stretch">
        A & R <br /> Business <br class="sm:hidden" /> Consultant
      </div>
      <div class="text-zinc-400 text-2xl font-semibold leading-10">
        Your Partner in Financial Growth and Stability!
      </div>
      <div
        class="text-slate-700 text-sm font-bold leading-5 self-stretch whitespace-nowrap mt-4 max-md:max-w-full"
      >
        Know more
      </div>
    </div>
    <!-- Social Icons -->
    <div
      class="flex max-w-full items-stretch gap-3 self-start max-md:justify-center max-md:mt-10"
    >
      <!-- <div
      class="justify-center items-center border border-[color:var(--AR-Gry,#314259)] flex shrink-0 h-[42px] flex-col flex-1 rounded-full border-solid"
    >
      <img src="/socials/fb.svg" alt="Facebook Logo" class="scale-75" />
    </div> -->
      <!-- <div
      class="justify-center items-center border border-[color:var(--AR-Gry,#314259)] flex shrink-0 h-[42px] flex-col flex-1 rounded-full border-solid"
    >
      <img src="/socials/ig.svg" alt="Instagram Logo" />
    </div> -->
      <div
        class="justify-center items-center flex shrink-0 flex-1 rounded-full md:p-2 ring-2 ring-[#314259]"
      >
        <a
          href="https://www.linkedin.com/company/a-r-business-consultant-limited"
          target="_blank"
          ><img
            src="/socials/in.svg"
            alt="Linkedin Logo"
            class="scale-75 md:scale-110"
          /></a
        >
      </div>
      <!-- <div
      class="justify-center items-center border border-[color:var(--AR-Gry,#314259)] flex shrink-0 h-[42px] flex-col flex-1 rounded-full border-solid"
    >
      <img src="/socials/x.svg" alt="Twitter Logo" />
    </div> -->
    </div>
  </div>
{/if}
