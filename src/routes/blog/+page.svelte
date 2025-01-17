<script>
  import BlogLink from '$lib/components/BlogLink.svelte';
  import Emulation from '$lib/assets/emulation.jpg';
  import Rss from '$lib/assets/rss.gif';
</script>

<svelte:head>
  <title>R0mZ (Da Blog) | Author Michael V. Colianna</title>
</svelte:head>

<h1>ROMs Central (aka Da Blog)</h1>

<div>
  <img
    alt="Several old video game systems."
    src={Emulation}
    height="268"
    widht="626"
  />
</div>

<p>
  This is my blog page. You didn't really think I was going to have ROMs here,
  right?
</p>

<p>
  Way back in the old days (literally, like 1998) my site had ROMs so I thought
  it'd be funny to name it like this. Sorry to disappoint!
</p>

<ul id="blog">
  <BlogLink date="2025-01-17" href="/my-first-post" isNew={true}
    >My first post</BlogLink
  >
</ul>

<div>
  <a href="/feed.xml">
    <img alt="Subscribe via RSS." src={Rss} height="15" width="80" />
  </a>
</div>

<div id="ending"></div>

<style>
  #blog {
    display: grid;
    gap: var(--spacing);
  }

  #ending {
    clear: both;
    padding-bottom: var(--spacing);
  }
</style>
