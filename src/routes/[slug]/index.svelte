<script context="module">
  export function preload (page) {
    return {
      details: {
        page: page.params.slug
      }
    }
  }
</script>

<script>
  import Inner from '../../components/Inner.svelte'
  export let details
</script>

<h3>this is buggy!</h3>
<p>The following should display current page. It <strong>doesn't</strong> change when the route change using anchor link click</p>

<Inner {details} />
