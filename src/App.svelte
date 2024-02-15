<script>
  import { Route, Router } from "svelte-navigator";
  import Hero from "./pages/Hero.svelte";
  import About from "./pages/About.svelte";
  import ServicesSection from "./pages/Services.svelte";
  import Testimonials from "./pages/Testimonials.svelte";
  import Navbar from "./pages/Navbar.svelte";
  import Footer from "./pages/Footer.svelte";

  import Services from "./pages/servicepage.svelte"
  import Connect from "./pages/connect.svelte";
  import AboutPage from "./pages/AboutPage.svelte";
</script>

<Router>
  <Route path="/" id="home">
    <div class="bg-white flex flex-col overflow-hidden">
      <Navbar />
      <Hero />
      <About />
      <ServicesSection />
      <Testimonials />
      <Footer />
    </div>
  </Route>
  <Route path="/about" component={AboutPage}></Route>
  <Route path="/services/:idx" let:params> <Services serviceIdx={params.idx}/> </Route>
  <Route path="/connect" component={Connect}></Route>
</Router>

<style>
</style>
