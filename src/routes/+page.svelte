<script>
  import Aim from '$lib/assets/aim.gif';
  import Blog from '$lib/assets/blog.png';
  import Bsky from '$lib/assets/bsky.gif';
  import Construction from '$lib/assets/construction.gif';
  import Emailme from '$lib/assets/emailme.gif';
  import ExternalLink from '$lib/components/ExternalLink.svelte';
  import Icq from '$lib/assets/icq.gif';
  import Indiosyncrasy from '$lib/assets/indiosyncrasy.jpg';
  import Mchammer from '$lib/assets/mchammer.gif';
  import Ring from '$lib/assets/ring.gif';
</script>

<svelte:head>
  <title>Author Michael V. Colianna's site</title>
</svelte:head>

<h1>Author Michael V. Colianna's site</h1>

<div>
  <img
    alt="Tacky clipart indicating under construction."
    src={Construction}
    height="51"
    width="574"
  />
</div>

<p>Welcome to my site! It is a work in progress so please excuse our dust!</p>

<p id="blog">
  <img alt="" src={Blog} height="64" width="64" />
  <a href="/blog/upgrading-oh-yeah/">Check out my latest blog post!</a>
</p>

<div id="hammer">
  <img alt="MC Hammer dancing." src={Mchammer} height="82" width="56" />
  <img aria-hidden="true" alt="" src={Mchammer} height="82" width="56" />
  <img aria-hidden="true" alt="" src={Mchammer} height="82" width="56" />
</div>

<p>
  <strong>YES, that's right, kids:</strong> My site has officially gone "old school".
  Now if I could just get the Sugar Hill Gang over here, maybe I could be "hip-hop"
  as well? Time to keep dreaming.
</p>

<p class="centerimg">
  <ExternalLink
    href="https://indiosyncrasy.com/authorfeature-michaelvcolianna/"
  >
    <img
      alt="I'm featured on Indiosyncrasy - for lovers of reading, writing, and discovery."
      src={Indiosyncrasy}
      height="212"
      width="470"
    />
  </ExternalLink>
</p>

<p class="centerimg">
  <ExternalLink href="https://runwithskizzers.neocities.org/web-ring">
    <img
      alt="Neocities official author web ring."
      src={Ring}
      height="313"
      width="313"
    />
    Check out this other cool web ring!
  </ExternalLink>
</p>

<p>There are a few ways to get in touch with me:</p>

<ul>
  <li>
    <img class="floaty" alt="Email." src={Emailme} height="50" width="50" />
    <strong>info@mvc.ink</strong>
  </li>

  <li>
    <img class="floaty" alt="ICQ." src={Icq} height="50" width="50" />
    <strong>7029668</strong> (found it in an old notebook, but ICQ is gone)
  </li>

  <li>
    <img
      class="floaty"
      alt="AOL Instant Messenger."
      src={Aim}
      height="50"
      width="50"
    />
    <strong>MekinWakko</strong> (true facts from back in the day!)
  </li>

  <li>
    <img class="floaty" alt="Bluesky." src={Bsky} height="50" width="50" />
    <strong
      ><ExternalLink href="https://bsky.app/profile/mvc.ink"
        >@mvc.ink</ExternalLink
      ></strong
    >
  </li>
</ul>

<div class="clearfix"></div>

<style>
  #blog {
    align-items: center;
    display: flex;
    gap: var(--spacing);
  }

  #hammer {
    display: flex;
    margin: auto;
    width: 168px;
  }

  ul {
    display: grid;
    gap: var(--spacing);
  }

  li {
    clear: both;
  }

  .floaty {
    float: left;
    margin-right: calc(var(--spacing) * 0.5);
  }

  .centerimg {
    text-align: center;
  }

  .centerimg img {
    margin: auto;
  }

  .clearfix {
    padding-top: calc(var(--spacing) * 2);
  }
</style>
