<script>
    export let heading, caption;
</script>

<div class="flex flex-col items-stretch w-3/12 ml-5 max-md:w-full max-md:ml-0 hover:scale-105 active:scale-105 focus:scale-105  transition-all ease-in duration-150">
    <div
        class="bg-stone-50 flex grow flex-col items-stretch container mx-auto px-7 py-11 rounded-3xl hover:ring-2 ring-gradient hover:ring-blue-600 max-md:mt-5 max-md:px-5 w-3/4 sm:w-full gradient-ring"
    >
        <img
            loading="lazy"
            src="https://cdn.builder.io/api/v1/image/assets/TEMP/8173a7b7-28bc-4e7f-b376-8274197ca2ef?apiKey=ebc3295e48c043a5ac0a48a737c5098e&"
            class="aspect-[1.08] object-contain object-center w-16 overflow-hidden self-center max-w-full"
            alt=""
        />
        <div
            class="text-slate-700 text-center text-3xl font-bold leading-1z1z self-center  mt-10"
        >
            { heading }
        </div> 
        <div
            class="text-zinc-400 text-center text-sm font-medium leading-6 mt-2.5"
        >
            { caption }
        </div>
    </div>
</div>
