<script>
  import ExternalLink from '$lib/components/ExternalLink.svelte';
  import Fcoe from '$lib/assets/fcoe.jpg';
  import Hot from '$lib/assets/hot.gif';
</script>

<svelte:head>
  <title>Stories | Author Michael V. Colianna</title>
</svelte:head>

<h1>MVC's stories</h1>

<div>
  <img
    alt="Cover artwork for Fractured Children of Earth. (Cropped.)"
    src={Fcoe}
    height="313"
    width="626"
  />
</div>

<p>
  <img class="floaty" alt="HOT" src={Hot} />
  That's part of the cover of my book, <ExternalLink
    href="https://bookshop.org/p/books/fractured-children-of-earth-michael-v-colianna/20609336"
    >Fractured Children of Earth</ExternalLink
  >! The cover is by <ExternalLink href="https://www.artofashesamuels.com/"
    >Ashe Samuels</ExternalLink
  >.
</p>

<p>
  Tagline: <strong
    >When a Deaf smuggler and her partner stumble upon a universe-wide
    conspiracy, getting humanity to understand the threat proves tougher than
    achieving their dreams of having a child.</strong
  >
</p>

<p>Detail:</p>

<blockquote>
  <p>
    Mary and her co-captain Davi are ready to retire and start a family. While
    smuggling’s been a profitable business, it’s also been filled with risk and
    uncertainty. They’re having trouble conceiving, though, so they have to keep
    going a little longer: The fertility procedures they need don’t come cheap.
  </p>
  <p>
    When a simple job inexplicably goes wrong, Mary gets shot and it throws
    their plans askew. But it’s not because they won’t get paid or even because
    the injury means more expensive treatments. It’s because Mary’s attackers
    are part of a fascist shadow government that’s dangerously close to bringing
    humanity under its thumb… and Davi recognizes them from the abusive
    childhood he fled.
  </p>
  <p>
    Mary and Davi want to warn humanity about what they’ve found, but their
    evidence is flimsy, they’re out of money, and other smugglers are hesitant
    to risk arrest for such an outlandish story. If they can’t convince anybody
    to help expose the plot and fight back, there might not be a free universe
    for anyone to live in—let alone for them to start the family they
    desperately desire.
  </p>
</blockquote>

<p>
  <em
    >For fans of the "Wayfarers" series by Becky Chambers, the "Expanse" series
    by James S.A. Corey, and the "Andor" television show.</em
  >
</p>

<div id="ending"></div>

<style>
  .floaty {
    float: left;
    margin-right: calc(var(--spacing) * 0.5);
  }

  blockquote {
    border-left: 2px solid var(--color-white);
    margin: 0;
    padding-left: calc(var(--spacing) * 2);
  }

  #ending {
    padding-bottom: var(--spacing);
  }
</style>
