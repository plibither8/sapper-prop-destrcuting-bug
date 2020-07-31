<script>
  // Extracted `page` varaible after destructuring `details`
  // does not get updated when the route changes
  // but accessing it directly: `details.page` works
  export let details
  const {page} = details
</script>

<h1>buggy, doesn't change</h1>

<!-- THIS LINE -->
<h2>This page is <strong>{page}</strong></h2>

<code>export let details;</code>
<code>{`const {page} = details;`}</code>
<code>...</code>
<code>{'<p>{page}</p>'}</code>

<br>
<br>
<br>

<h1>fixed, does change</h1>

<!-- AND THIS LINE -->
<h2>This page is <strong>{details.page}</strong></h2>

<code>export let details;</code>
<code>...</code>
<code>{'<p>{details.page}</p>'}</code>

<style>
  code {
    display: block;
  }
</style>
