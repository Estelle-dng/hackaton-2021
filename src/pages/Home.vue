<template>
  <div class="app">
    <header>
      <Navbar />
    </header>
    <main>
      <Hero />
    </main>
    <footer>
      <Footer />
    </footer>
  </div>
</template>

<script>
import Navbar from "@/components/Navbar";
import Hero from "@/modules/Hero";
import Footer from "@/components/Footer";
export default {
  name: "Home",
  components: {
    Navbar,
    Hero,
    Footer,
  },
};
</script>

<style></style>
