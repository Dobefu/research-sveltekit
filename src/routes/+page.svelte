<script>
  let count = $state(0)
</script>

<svelte:head>
  <title>Home | Research - SvelteKit</title>
  <meta name="description" content="Description" />
</svelte:head>

<h1 class="text-3xl font-medium">Research - SvelteKit</h1>

<p class="py-4">Count: {count}</p>

<button class="rounded-md px-4 py-2 bg-gray-200" onclick={() => count--}>
  Decrement
</button>

<button
  class="rounded-md px-4 py-2 bg-red-200 disabled:bg-gray-100"
  disabled={count === 0}
  onclick={() => (count = 0)}
>
  Reset
</button>

<button class="rounded-md px-4 py-2 bg-gray-200" onclick={() => count++}>
  Increment
</button>
