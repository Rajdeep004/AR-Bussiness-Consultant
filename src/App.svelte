<script>
  import { Route, Router } from "svelte-navigator";
  import Hero from "./pages/Hero.svelte";
  import About from "./pages/About.svelte";
  import ServicesSection from "./pages/Services.svelte";
  import Testimonials from "./pages/Testimonials.svelte";
  import Navbar from "./pages/Navbar.svelte";
  import Footer from "./pages/Footer.svelte";

  import services from "./pages/servicepage.svelte"
  import Connect from "./pages/connect.svelte";
</script>

<Router>
  <Route path="/" id="home">
    <div class="bg-white flex flex-col sm:pt-8 overflow-hidden">
      <Navbar />
      <Hero />
      <About />
      <ServicesSection />
      <Testimonials />
      <Footer />
    </div>
  </Route>
  <Route path="/services" component={services}></Route>
  <Route path="/connect" component={Connect}></Route>
</Router>

<style>
</style>
