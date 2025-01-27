<script>
  import ExternalLink from '$lib/components/ExternalLink.svelte';
  import Globe from '$lib/assets/globe.png';
</script>

<svelte:head>
  <title>Links | Author Michael V. Colianna</title>
</svelte:head>

<h1>Lanks</h1>

<div>
  <img
    id="globe"
    alt="Tacky clipart of a globe with a search bar wrapping around it, with a pointer icon."
    src={Globe}
    height="216"
    width="260"
  />
</div>

<p>
  These are some cool pages you should check out! Come back here often, as this
  list will grow.
</p>

<ul>
  <li>
    <ExternalLink href="https://fiyahlitmag.com/">FIYAH</ExternalLink> - An awesome
    spec fic magazine.
  </li>

  <li>
    <ExternalLink
      href="https://gregpak.com/how-and-why-to-make-a-personal-website/"
      >How to (and why you should) make a personal website</ExternalLink
    > - Great guide by Greg Pak!
  </li>

  <li>
    <ExternalLink href="https://kiwisbybeat.net/">Kiwis By Beat!</ExternalLink> -
    A fan archive of comics by Ryan Armand, the creator of "minus."
  </li>

  <li>
    <ExternalLink href="https://indiosyncrasy.com/">Indiosyncrasy</ExternalLink>
    - A great site with reviews & profiles for indie authors.
  </li>

  <li>
    <ExternalLink href="https://ooh.directory/">ooh.directory</ExternalLink> - An
    awesome directory of blogs on all kinds of topics!
  </li>

  <li>
    <ExternalLink href="https://runwithskizzers.neocities.org/"
      >Preeti Chhibber</ExternalLink
    >
    - Preeti is the one who pointed out NeoCities &amp; got me excited to make this
    old school site.
  </li>

  <li>
    <ExternalLink href="https://startingoffwrite.com/"
      >Starting Off Write</ExternalLink
    >
    - A cool writing group I joined to help motivate me.
  </li>

  <li>
    <ExternalLink
      href="https://www.webdesignmuseum.org/exhibitions/web-banners-in-the-90s"
      >Web Banners in the 90s</ExternalLink
    > - Did you get a kick out of my footer? Thank these folks!
  </li>
</ul>

<div id="ending"></div>

<style>
  #globe {
    margin: auto;
  }

  li {
    margin: 18px 0;
  }

  #ending {
    padding-bottom: var(--spacing);
  }
</style>
