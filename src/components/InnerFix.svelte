<script>
  export let details
</script>
<!-- 
  But when accessed directly from the `details` object
  it works as it should, updating on route change
-->
<h1>This page is: <strong>{details.page}</strong></h1>
