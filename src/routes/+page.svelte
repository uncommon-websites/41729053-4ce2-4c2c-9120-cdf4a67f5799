<script lang="ts">
  import Header from "$lib/components/Header.svelte";
  import Hero from "$lib/components/Hero.svelte";
  import Stats from "$lib/components/Stats.svelte";
  import WhyAttend from "$lib/components/WhyAttend.svelte";
  import Passes from "$lib/components/Passes.svelte";
  import Speakers from "$lib/components/Speakers.svelte";
  import WhyNow from "$lib/components/WhyNow.svelte";
  import Agenda from "$lib/components/Agenda.svelte";
  import FAQ from "$lib/components/FAQ.svelte";
  import Footer from "$lib/components/Footer.svelte";
</script>

<main class="bg-[#101010] min-h-screen font-sans text-[#FCFCFC] selection:bg-[#3B51E1] selection:text-white">
  <Header />
  <Hero />
  <Stats />
  <WhyAttend />
  <Passes />
  <Speakers />
  <WhyNow />
  <Agenda />
  <FAQ />
  <Footer />
</main>

