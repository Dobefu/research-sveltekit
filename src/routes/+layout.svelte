<script>
  import '../app.css'
  import Header from '../components/layout/Header.svelte'
  import Footer from '../components/layout/Footer.svelte'
</script>

<Header />

<main class="px-8 flex-1" id="main-content">
  <slot />
</main>

<Footer />
