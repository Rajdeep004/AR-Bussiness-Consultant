<script>
import { createEventDispatcher } from "svelte"
export let idx,heading,caption,isSelected;

const dispatch = createEventDispatcher();

const updateContent = ()=>{
  dispatch("addIdx",idx)
}
</script>

<div
  class={`bg-stone-50 flex flex-col items-stretch justify-start container mx-auto px-7 py-8 rounded-3xl hover:ring-2 ring-gradient hover:ring-blue-600 max-md:mt-5 max-md:px-5 gradient-ring hover:scale-105 active:scale-105 focus:scale-105 transition-all ease-in duration-150 max-w-[35vh] cursor-pointer  ${isSelected ? "!bg-blue-600/95 !text-white" : ""}`}
  on:click={updateContent}
>
  <div class={` text-3xl font-bold self-center ${isSelected ? "text-slate-100" : "text-slate-700"}`}>
    {heading}
  </div>
  <div class={`text-md font-medium leading-6 mt-2.5 ${isSelected?"text-zinc-100":"text-zinc-400"}`}>
    {caption}
  </div>
  <div class="flex items-center max-w-full gap-2 w-full justify-between">
    <a href="#f" class="underline mt-4">Know More</a>
    <img
      loading="lazy"
      class="w-16 overflow-hidden self-end"
      src="https://cdn.builder.io/api/v1/image/assets/TEMP/8173a7b7-28bc-4e7f-b376-8274197ca2ef?apiKey=ebc3295e48c043a5ac0a48a737c5098e&"
      alt="service icon"
    />
  </div>
</div>
