<script>
  import globe from '$lib/assets/globe.png';
  import ring from '$lib/assets/ring.gif';
</script>

<svelte:head>
  <title>Links | Author Michael V. Colianna</title>
</svelte:head>

<h1>Lanks</h1>

<div>
  <img id="globe" alt="Tacky clipart of a globe with a search bar wrapping around it, with a pointer icon." src={globe} />
</div>

<p>
  <a href="https://runwithskizzers.neocities.org/web-ring" rel="noopener noreferrer">
    <img alt="Neocities official author web ring." src={ring} />
    Check out the web ring!
  </a>
</p>

<style>
  #globe {
    margin: auto;
    width: 260px;
  }
</style>