<script>
    import {about} from "../content.js"
    import Footer from "./Footer.svelte";
    import Navbar from "./Navbar.svelte";
</script>
<Navbar />
<div class="mb-8">
    <section
      id="AboutUS"
      class="flex flex-col px-6 py-8 gap-4 justify-center items-center"
    >
    <div class={`flex items-center flex-col lg:flex-row`}>
      <img
        loading="lazy"
        src="https://cdn.builder.io/api/v1/image/assets/TEMP/a145f476-4deb-4698-a63a-efe1ad3227e1?apiKey=ebc3295e48c043a5ac0a48a737c5098e&"
        class="aspect-square object-contain object-center w-3/4 lg:w-48 overflow-hidden self-center shrink-0 max-w-full my-auto"
        alt=""
      />
      <p
        class={`max-w-4xl font-medium text-justify selection:bg-blue-600 selection:text-black`}
        
      > {about[0]} {about[1]} </p>
    </div>
    <div class={`flex items-center flex-col lg:flex-row-reverse`}>
      <img
        loading="lazy"
        src="https://cdn.builder.io/api/v1/image/assets/TEMP/a145f476-4deb-4698-a63a-efe1ad3227e1?apiKey=ebc3295e48c043a5ac0a48a737c5098e&"
        class="aspect-square object-contain object-center w-3/4 lg:w-48 overflow-hidden self-center shrink-0 max-w-full my-auto"
        alt=""
      />
      <p
        class={`max-w-4xl font-medium text-justify selection:bg-blue-600 selection:text-black`}
      > {about[2]} {about[3]}</p>
    </div>
    <div class={`flex items-center flex-col lg:flex-row`}>
      <img
        loading="lazy"
        src="https://cdn.builder.io/api/v1/image/assets/TEMP/a145f476-4deb-4698-a63a-efe1ad3227e1?apiKey=ebc3295e48c043a5ac0a48a737c5098e&"
        class="aspect-square object-contain object-center w-3/4 lg:w-48 overflow-hidden self-center shrink-0 max-w-full my-auto"
        alt=""
      />
      <p
        class={`max-w-4xl font-medium text-justify selection:bg-blue-600 selection:text-black`}
        
      > {about[4]} {about[5]} </p>
    </div>
    </section>
</div>
<Footer />