<script>
  import ExternalLink from '$lib/components/ExternalLink.svelte';
  import '../app.css';

  let { children } = $props();
</script>

<svelte:head>
  <meta name="robots" content="noai, noimageai" />
</svelte:head>

<div class="wrap">
  <header>
    <div class="logo">
      <div>mvc</div>
      <div id="ink">.ink</div>
    </div>

    <hr />

    <nav>
      <a href="/">main</a>
      <a href="/stories">stories</a>
      <a href="/about">about</a>
      <a href="/roms">roms</a>
      <a href="/links">links</a>
    </nav>

    <hr />

    <div class="copyright">
      <div>&copy; 2025</div>
      <div>mvc.ink</div>
    </div>

    <a href="mailto:info@mvc.ink">contact</a>
  </header>

  <main>
    {@render children()}

    <div id="counter">
      <ExternalLink href="https://www.free-website-hit-counter.com"
        ><img
          src="https://www.free-website-hit-counter.com/zc.php?d=6&id=3561&s=1"
          border="0"
          alt="Free Website Hit Counter"
          id="counter-image"
        /></ExternalLink
      >
      <br />
      <small
        ><ExternalLink href="https://www.free-website-hit-counter.com"
          >Free website hit counter</ExternalLink
        ></small
      >
    </div>
  </main>
</div>

<style>
  .wrap {
    display: grid;
    grid-template-columns: 1fr 84px;
    gap: 12px;
    margin: auto;
    max-width: 626px;
  }

  header {
    background-color: var(--color-olive);
    font-weight: bold;
    min-height: 85vh;
    order: 2;
    padding: 12px;
    text-align: center;
  }

  .logo {
    font-size: 28px;
  }

  #ink {
    color: var(--color-white);
    -webkit-text-stroke: 2px var(--color-black);
    text-transform: uppercase;
  }

  hr {
    border-color: var(--color-forest);
    border-style: solid;
  }

  nav {
    display: grid;
    gap: 12px;
  }

  a {
    align-items: center;
    display: flex;
    color: var(--color-black);
    height: 20px;
    justify-content: center;
  }

  .copyright {
    font-size: 18px;
    margin-bottom: 6px;
  }

  main {
    order: 1;
  }

  #counter {
    margin-top: 24px;
    text-align: center;
  }

  #counter-image {
    margin: auto;
  }
</style>
