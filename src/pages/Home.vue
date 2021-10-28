<template>
  <div class="app">
    <header>
      <Navbar />
    </header>
    <main>
      <Hero />
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
import Footer from "@/components/Footer";
export default {
  name: "Home",
  components: {
    Navbar,
    Hero,
    Footer,
    Partners,
    Newsletter,
  },
};
</script>

<style></style>
