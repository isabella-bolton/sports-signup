<script>
  let name = "";
</script>

<style>
  /* ####### LAYOUT ####### */
  section {
    display: grid;
    grid-gap: 50px;
    grid:
      " .       .              .            nav          nav         " auto
      " dancer  relayrunner    basketballer hockeyplayer .           " auto
      " header  header         header       header       header      " 215px
      / 1fr 1fr 1fr 1fr 1fr;
  }

  header {
    grid-area: header;
  }
  nav {
    grid-area: nav;
  }
  #dancer {
    grid-area: dancer;
  }
  #relayrunner {
    grid-area: relayrunner;
  }
  #basketballer {
    grid-area: basketballer;
  }
  #hockeyplayer {
    grid-area: hockeyplayer;
  }

  /* ######## STYLE ####### */

  #hockeyplayer {
    margin-top: 50px;
  }

  #dancer {
    margin-top: 70px;
    margin-left: 130px;
  }

  nav {
    margin-top: 50px;
  }

  img {
    width: 200px;
  }

  header {
    background-color: #1e387c;
    border-top: 8px solid #ffc600;
  }
</style>

<section>

  <header>
    <h1 class="title is-1 title has-text-centered has-text-warning">
      Rangi Ruru Weekly Basketball Signup
    </h1>
  </header>

  <nav>
    <input bind:value={name} placeholder="Name" />

    {#if name}
      <p>Hello {name}</p>
    {:else}
      <p>Please enter your name.</p>
    {/if}

    <a class="button" href="teams">Next</a>
  </nav>

  <img id="dancer" src="/Dancer.png" alt="Dancer" />
  <img id="relayrunner" src="/Relay.png" alt="Relay runner" />
  <img id="basketballer" src="/Basketball.png" alt="Basketballer" />
  <img id="hockeyplayer" src="/Hockey.png" alt="Hockey player" />

</section>
