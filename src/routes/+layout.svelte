<script>
  import ExternalLink from '$lib/components/ExternalLink.svelte';
  import IeLogo from '$lib/assets/ie-logo.gif';
  import MvcTitle from '$lib/assets/mvc-title.png';
  import NavLink from '$lib/components/NavLink.svelte';
  import Neocities from '$lib/assets/neocities.png';
  import Noframes from '$lib/assets/noframes.gif';
  import Notepad from '$lib/assets/notepad.gif';
  import NsLogo from '$lib/assets/ns-logo.gif';
  import { onMount } from 'svelte';
  import { page } from '$app/state';
  import { PUBLIC_APP_MODE } from '$env/static/public';
  import Quicktime from '$lib/assets/quicktime.gif';
  import '../app.css';

  let { children } = $props();

  const links = [
    { href: '/', label: 'Main page' },
    { href: '/about', label: 'About me' },
    { href: '/stories', label: 'My stories' },
    { href: '/blog', label: 'ROMs central' },
    { href: '/links', label: 'Cool links' }
  ];

  const building = PUBLIC_APP_MODE === 'prod';

  let bannerAd;

  const images = import.meta.glob('../../static/banners/*');
  const bannerAds = Object.keys(images);

  onMount(() => {
    const bannerAdSrc = bannerAds[Math.floor(Math.random() * bannerAds.length)];

    bannerAd.src = bannerAdSrc.replace('../../static', '');
  });
</script>

<svelte:head>
  <meta
    property="og:description"
    content="The super cool old school website for author Michael V. Colianna."
  />
  <meta
    property="og:image"
    content="https://michaelcolianna.neocities.org/mvc-og.png"
  />
  <meta name="robots" content="noai, noimageai" />
</svelte:head>

<a href="#content">Skip to content</a>

<div class="wrap">
  <header>
    <img alt="Michael V. Colianna." src={MvcTitle} height="188" width="626" />

    <nav>
      {#each links as link}
        <NavLink {link} />
      {/each}
    </nav>
  </header>

  <main id="content">
    {@render children()}

    <div id="icons">
      <img alt="Internet Explorer badge." src={IeLogo} height="31" width="88" />
      <img alt="Netscape Navigator badge." src={NsLogo} height="31" width="88" />
      <img
        alt="Campaign against frames badge."
        src={Noframes}
        height="31"
        width="87"
      />
      <img alt="Made with Notepad badge." src={Notepad} height="31" width="82" />
      <img alt="Quicktime badge." src={Quicktime} height="31" width="88" />
      <img
        alt="Hosted by Neocities badge."
        src={Neocities}
        height="31"
        width="105"
      />
    </div>

    {#if building}
      <div id="counter">
        <ExternalLink href="https://www.free-website-hit-counter.com"
          ><img
            src="https://www.free-website-hit-counter.com/zc.php?d=6&id=3561&s=1"
            border="0"
            alt="Free Website Hit Counter."
            id="counter-image"
          /></ExternalLink
        >

        <small
          ><ExternalLink href="https://www.free-website-hit-counter.com"
            >Free website hit counter</ExternalLink
          ></small
        >
      </div>
    {/if}
  </main>

  <footer>
    <div class="copyright">
      &copy; 2017-{new Date().getFullYear()} - Michael V. Colianna -
      <a href="mailto:info@mvc.ink">Contact</a>
    </div>
  </footer>

  <div id="fake-banner-ad">
    <span>Fake banner ad:</span>
    <img bind:this={bannerAd} alt="A random, fake banner ad." src />
  </div>
</div>

<style>
  [href='#content'] {
    background-color: var(--color-black);
    color: var(--color-white);
    left: -9999px;
    opacity: 0;
    padding: var(--spacing);
    position: absolute;
    z-index: 999;
  }

  [href='#content']:focus {
    left: var(--spacing);
    opacity: 1;
    transform: translateX(var(--spacing));
  }

  .wrap {
    margin: auto;
    max-width: 626px;
  }

  header {
    display: grid;
    gap: var(--spacing);
  }

  nav {
    background-color: var(--color-black);
    border: 1px solid var(--color-white);
    box-shadow: 0 0 2px 2px var(--color-grey);
    display: flex;
    flex-wrap: wrap;
    justify-content: space-evenly;
  }

  #icons {
    display: flex;
    flex-wrap: wrap;
    gap: calc(var(--spacing) * 0.5);
    margin-bottom: var(--spacing);
  }

  footer {
    align-items: center;
    background-color: var(--color-black);
    border: 1px solid var(--color-white);
    box-shadow: 0 0 2px 2px var(--color-grey);
    display: flex;
    height: calc(var(--spacing) * 3);
    margin-bottom: calc(var(--spacing) * 2);
    padding: 0 var(--spacing);
  }

  #counter {
    margin-bottom: 24px;
    margin-top: 24px;
    text-align: center;
  }

  #counter-image {
    margin: auto;
  }

  #fake-banner-ad {
    font-size: calc(var(--spacing) * 0.75);
    margin-bottom: var(--spacing);
    min-height: 75px;
    text-align: center;
  }

  #fake-banner-ad span {
    display: block;
    margin-bottom: calc(var(--spacing) * 0.5);
  }

  #fake-banner-ad img {
    margin: auto;
  }
</style>
