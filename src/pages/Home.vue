<template>
  <div class="app">
    <header>
      <Navbar />
    </header>
    <main>
      <Hero />
      <StepsBloc />
      <Partners />
      <About />
      <Newsletter />
    </main>
    <footer>
      <Footer />
    </footer>
  </div>
</template>

<script>
import Navbar from "@/components/Navbar";
import Hero from "@/modules/Hero";
import Partners from "@/modules/Partners";
import Newsletter from "@/modules/Newsletter";
import StepsBloc from "@/modules/StepsBloc";
import About from "@/modules/About";
import Footer from "@/components/Footer";
export default {
  name: "Home",
  components: {
    Navbar,
    Hero,
    Footer,
    Partners,
    Newsletter,
    StepsBloc,
    About
  },
};
</script>

<style></style>
