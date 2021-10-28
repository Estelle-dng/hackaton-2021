<template>
  <div class="app">
    <header>
      <Navbar />
    </header>
    <main>
      <Hero />
      <StepsBloc />
      <Partners />
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
import Footer from "@/components/Footer";
export default {
  name: "Home",
  components: {
    Navbar,
    Hero,
    Footer,
    Partners,
    Newsletter,
    StepsBloc
  },
};
</script>

<style></style>
