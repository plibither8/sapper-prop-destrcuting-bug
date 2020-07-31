<script>
  // Extracted `page` varaible after destructuring `details`
  // does not get updated when the route changes
  // but accessing it directly: `details.page` works
  export let details
  const {page} = details
</script>

<h2>buggy, doesn't change</h2>

<!-- THIS LINE -->
<h1>This page is <strong>{page}</strong></h1>

<code>export let details;</code>
<code>{`const {page} = details;`}</code>
<code>...</code>
<code>{'<p>{page}</p>'}</code>

<br>
<br>
<br>

<h2>fixed, does change</h2>

<!-- AND THIS LINE -->
<h1>This page is <strong>{details.page}</strong></h1>

<code>export let details;</code>
<code>...</code>
<code>{'<p>{details.page}</p>'}</code>

<style>
  code {
    display: block;
  }
</style>
