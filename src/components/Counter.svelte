<script>
  let count = $state(0)
</script>

<div class="border p-4 inline-flex flex-col shadow-lg rounded-2xl">
  <p class="pb-4 mx-auto">Count: {count}</p>

  <div class="flex gap-4">
    <button
      class="transition-colors rounded-md px-4 py-2 bg-gray-200 hover:bg-gray-300 shadow"
      onclick={() => count--}
    >
      Decrement
    </button>

    <button
      class="transition-all rounded-md px-4 py-2 bg-red-200 disabled:bg-gray-100 disabled:text-gray-500 shadow disabled:shadow-none"
      disabled={count === 0}
      onclick={() => (count = 0)}
    >
      Reset
    </button>

    <button
      class="transition-colors rounded-md px-4 py-2 bg-gray-200 hover:bg-gray-300 shadow"
      onclick={() => count++}
    >
      Increment
    </button>
  </div>
</div>
