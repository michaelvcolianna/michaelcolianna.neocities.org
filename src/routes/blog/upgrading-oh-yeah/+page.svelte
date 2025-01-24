<script>
  import BackLink from '$lib/components/BackLink.svelte';
  import BlogDate from '$lib/components/BlogDate.svelte';
  import ExternalLink from '$lib/components/ExternalLink.svelte';
  import NeocitiesUpgrade from '$lib/assets/r0mz/neocities-upgrade.jpg';
</script>

<BackLink />

<h1>UPGRADING: Oh Yeah!</h1>

<BlogDate date="2017-01-25" />

<p>
  <img
    alt="Screenshot of Michael's Neocities dashboard, showing his custom URL instead of the default Neocities one."
    src={NeocitiesUpgrade}
    height="191"
    width="626"
  />
</p>

<p>
  This is a short post but with super cool news: I became a supporter on
  Neocities, so now my custom domain points here. Instead of <code
    >https://michaelcolianna.neocities.org</code
  >
  you can just go right to <code>https://mvc.ink</code>!
</p>

<p>
  I also added a link to the FCoE appendix on the <a href="/stories"
    >stories page</a
  >!
</p>

<p>
  <em
    >Also, check out the source of the page to see the name of the folder I'm
    using for blog images. ;‑)</em
  >
</p>

<div class="ender"></div>
