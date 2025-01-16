<script>
  let { href, children } = $props();
</script>

<a {href} rel="noopener noreferrer">{@render children()}</a>
