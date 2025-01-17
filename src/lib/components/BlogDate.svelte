<script>
  let { date } = $props();

  const isoDate = new Date(date).toISOString();
</script>

<div>
  Posted <time datetime={isoDate}>{date}</time>
</div>

<style>
  time {
    font-style: italic;
  }
</style>
