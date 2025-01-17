<script>
  import Mvc from '$lib/assets/mvc.jpg';
</script>

<svelte:head>
  <title>About | Author Michael V. Colianna</title>
</svelte:head>

<h1>About MVC</h1>

<div aria-hidden="true">
  <img alt="" src={Mvc} height="260" width="260" />
</div>

<p>
  The image above is a 3/4 photograph of me, showing the taper of my beard and
  the shaved portion on the right of my head, as well as a peek of my teal hair.
</p>

<p>About:</p>

<blockquote>
  <p>
    Michael (he/him) is a hard-of-hearing/deaf author (and a web developer).
    Michael writes a mix of fantasy and science-fiction set in the distant
    future. His stories in either genre are grounded, focusing on the character
    relationships and societal changes instead of magical creatures or space
    battles. A current of mystery runs under them all, as well.
  </p>
  <p>
    The skeleton for Michael’s stories began forming as early as 14 years old.
    He wondered what the future held for humanity, and whether we would travel
    into space. Idolizing Ursula K. LeGuin, Isaac Asimov, and C.S. Friedman, he
    followed humanity into the future and a combination of science
    fiction/fantasy elements trickled into the resulting stories.
  </p>
  <p>
    Outside of writing, Michael bicycles, runs, and lifts weights. He’s also
    been running a Dungeons & Dragons campaign for over 20 years with his unruly
    and – let’s say imaginitive – friends. He and his wife were on a curious
    journey sparked by infertility as they tried to expand their family. As
    well, Michael has a condition that makes him hard-of-hearing and sometimes
    deaf. Those elements have found their ways into his stories.
  </p>
</blockquote>

<div id="ending"></div>

<style>
  img {
    background-color: var(--color-black);
    border: 2px solid var(--color-white);
    box-shadow: 0 0 2px 2px var(--color-grey);
    border-radius: 260px;
    margin: auto;
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
