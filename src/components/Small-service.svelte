<script>
  export let heading, caption;
</script>

<div
  class="flex flex-col items-stretch min-w-[25%] max-md:w-full max-md:ml-0 hover:scale-105 active:scale-105 focus:scale-105 transition-all ease-in duration-150"
>
  <div
    class="bg-stone-50 flex grow flex-col items-stretch container mx-auto px-7 py-8 rounded-3xl hover:ring-2 ring-gradient hover:ring-blue-600 max-md:mt-5 max-md:px-5 w-3/4 sm:w-full gradient-ring"
  >
    <div class="text-slate-700 text-c text-3xl font-bold self-center">
      {heading}
    </div>
    <div class="text-zinc-400 text- text-md font-medium leading-6 mt-2.5">
      {caption}
    </div>
    <div class="flex items-center max-w-full mt-6 gap-2 w-full justify-between">
      <a href="#f" class="underline mt-4">Know More</a>
      <img
        loading="lazy"
        class="w-16 overflow-hidden self-end"
        src="https://cdn.builder.io/api/v1/image/assets/TEMP/8173a7b7-28bc-4e7f-b376-8274197ca2ef?apiKey=ebc3295e48c043a5ac0a48a737c5098e&"
        alt="service icon"
      />
    </div>
  </div>
</div>
