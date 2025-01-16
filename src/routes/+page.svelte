<script>
  import ExternalLink from '$lib/components/ExternalLink.svelte';
  import construction from '$lib/assets/construction.gif';
  import ring from '$lib/assets/ring.gif';
</script>

<svelte:head>
  <title>Author Michael V. Colianna's site</title>
</svelte:head>

<h1>Author Michael V. Colianna's site</h1>

<div>
  <img alt="Tacky clipart indicating under construction." src={construction} />
</div>

<p>Welcome to my site! It is a work in progress so please excuse our dust!</p>

<p>
  <strong>YES, that's right, kids:</strong> My site has officially gone "old school".
  Now if I could just get the Sugar Hill Gang over here, maybe I could be "hip-hop"
  as well? Time to keep dreaming.
</p>

<p>This site probably looks best in Internet Explorer. (Kidding.)</p>

<p id="webring">
  <ExternalLink href="https://runwithskizzers.neocities.org/web-ring">
    <img alt="Neocities official author web ring." src={ring} />
    Check out the web ring!
  </ExternalLink>
</p>

<p>There are a few ways to get in touch with me:</p>

<ul>
  <li>Email: <strong>info@mvc.ink</strong></li>
  <li>
    ICQ: <strong>7029668</strong> (found it in an old notebook, but ICQ is gone)
  </li>
  <li>
    AOL Instant Messenger: <strong>MekinWakko</strong> (true facts from back in the
    day!)
  </li>
  <li>
    Bluesky: <strong
      ><ExternalLink href="https://bsky.app/profile/mvc.ink"
        >@mvc.ink</ExternalLink
      ></strong
    >
  </li>
</ul>

<style>
  img {
    margin: auto;
    width: 260px;
  }

  #webring {
    text-align: center;
  }
</style>
