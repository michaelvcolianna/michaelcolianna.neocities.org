<script>
  import { page } from '$app/state';

  let { link } = $props();

  const { href, label } = link;
</script>

<a {href} aria-current={page.url.pathname === href ? 'page' : undefined}
  >{label}</a
>

<style>

a {
    align-items: center;
    display: flex;
    height: calc(var(--spacing) * 3);
    justify-content: center;
    padding: 0 var(--spacing);
  }
</style>
