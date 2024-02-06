<script>
  import Footer from "./Footer.svelte";
  import Navbar from "./Navbar.svelte";
  import * as RadioGroup from "../lib/components/ui/radio-group";
  import { Label } from "../lib/components/ui/label";
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
    <RadioGroup.Root>
      <div class="flex items-center space-x-2">
        <RadioGroup.Item value="Company" id="r1" />
        <Label for="r1">Company</Label>
      </div>
      <div class="flex items-center space-x-2">
        <RadioGroup.Item value="Sole trader" id="r2" />
        <Label for="r2">Sole trader</Label>
      </div>
      <div class="flex items-center space-x-2">
        <RadioGroup.Item value="Indiviual" id="r3" />
        <Label for="r3">Indiviual</Label>
      </div>
      <div class="flex items-center space-x-2">
        <RadioGroup.Item value="Patnership" id="r4" />
        <Label for="r4">Patnership</Label>
      </div>
      <RadioGroup.Input name="spacing" />
    </RadioGroup.Root>
    
  </div>
</section>
<Footer />
