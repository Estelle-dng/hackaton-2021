<template>
  <div class="app">
    <header>
      <wrapper>
        <Navbar />
      </wrapper>
    </header>
    <main>
      <wrapper>
        <Hero />
      </wrapper>
    </main>
    <footer>
        <Footer />
    </footer>
  </div>
</template>

<script>
import Navbar from "@/components/Navbar";
import Hero from "@/modules/Hero";
import Footer from "@/modules/Footer";
import Wrapper from "../components/Wrapper/Wrapper.vue";
export default {
  name: "Home",
  components: {
    Navbar,
    Hero,
    Footer,
    Wrapper,
  },
};
</script>

<style></style>
