<script>
  import "../app.css";
  import Header from '../components/layout/Header.svelte'
</script>

<Header />

<main class="px-8" id="main-content">
  <slot />
</main>
