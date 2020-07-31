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

<Inner {details} />
