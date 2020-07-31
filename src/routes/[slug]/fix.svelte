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
  import InnerFix from '../../components/InnerFix.svelte'
  export let details
</script>

<h3>this is fixed!</h3>
<p>The following should display current page. It <strong>does</strong> change when the route change using anchor link click</p>

<InnerFix {details} />
