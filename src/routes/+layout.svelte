<script>
  import "../app.css";
  import "tailwindcss/tailwind.css";
  import TopBar from "../components/TopBar.svelte";
  import Footer from "../components/Footer.svelte";
  import Faq from "../components/FAQ.svelte";
</script>

<TopBar />

<main>
  <slot />
</main>

<Faq />

<Footer />
