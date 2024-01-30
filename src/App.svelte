<script>
  import { Route, Router } from "svelte-navigator";
  import Header from "./pages/Hero.svelte";
  import ServicesSection from "./pages/Services.svelte";
  import Infographical from "./pages/About.svelte";
  import Testimonials from "./pages/Testimonials.svelte";
  import Navbar from "./pages/Navbar.svelte";
  import Footer from "./pages/Footer.svelte";

  import services from "./pages/servicepage.svelte"
</script>

<Router>
  <Route path="/" id="home">
    <div class="bg-white flex flex-col sm:pt-8 overflow-hidden">
      <Navbar />
      <Header />
      <Infographical />
      <ServicesSection />
      <Testimonials />
      <Footer />
    </div>
  </Route>
  <Route path="/services" component={services}></Route>
</Router>

<style>
</style>
