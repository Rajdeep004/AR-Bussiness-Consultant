<script>
    import {about} from "../content.js"
    import Footer from "./Footer.svelte";
    import Navbar from "./Navbar.svelte";
</script>
<Navbar />
<div class="bg-gradient-to-b sm:bg-gradient-to-r from-[#006FF2] to-[#004391] mb-8">
    <section
      id="AboutUS"
      class="flex flex-col px-6 py-8 gap-4 justify-center items-center"
    >
    {#each about as para}
      <p
        class="max-w-4xl font-medium text-white text-justify selection:bg-white selection:text-black"
      > {para} </p>
    {/each}
      
    </section>
</div>
<Footer />