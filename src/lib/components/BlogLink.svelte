<script>
  import New from '$lib/assets/new.gif';

  let { date, href, isNew, children } = $props();

  const isoDate = new Date(date).toISOString();
</script>

<li>
  {#if isNew}
    <img alt="New" src={New} height="21" width="32" />
  {/if}

  <time datetime={isoDate}>{date}</time>

  <a href={`/blog${href}`}>
    {@render children()}
  </a>
</li>

<style>
  img {
    clear: both;
    float: left;
    margin-right: calc(var(--spacing) * 0.5);
  }
</style>
