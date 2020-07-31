<script>
  export let details
  // Extracted `page` varaible after destructuring `details`
  // does not get updated when the route changes
  const {page} = details
</script>

<h1>This page is: <strong>{page}</strong></h1>
