<script>
  import Footer from "./Footer.svelte";
  import Navbar from "./Navbar.svelte";
</script>

<Navbar />
<section
  id="quotation"
  class="container mx-auto flex flex-col justify-center item-center bg-red-300"
>
  <h1 class="text-3xl font-bold text-center">Get a quotation</h1>
  <div>
    <input type="text" class="rounded-md" placeholder="Name" />
    <input type="text" class="rounded-md" placeholder="phone" />
    <input type="text" class="rounded-md" placeholder="email" />
    <h4 class="text-xl font-semibold">Type of orgaisation?</h4>

    <label for="org"
      ><input type="radio" name="org" value="Company" />Company</label
    >

    <label for="org"
      ><input type="radio" name="org" value="Sole trader" />Sole trader</label
    >

    <label for="org"
      ><input type="radio" name="org" value="Individual" />Individual</label
    >

    <label for="org"
      ><input type="radio" name="org" value="Patership" />Patnership</label
    >
  </div>
</section>
<Footer />
