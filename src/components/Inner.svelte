<script>
  // Extracted `page` varaible after destructuring `details`
  // does not get updated when the route changes
  // but accessing it directly: `details.page` works
  export let details
  const {page} = details
</script>

<svelte:head>
  <title>{page}</title>
</svelte:head>

<h1>(buggy, doesn't change) This page is: <strong>{page}</strong></h1>
<h1>(fixed, does change) This page is: <strong>{details.page}</strong></h1>
