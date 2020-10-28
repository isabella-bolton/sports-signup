<script>
  import { goto } from "@sapper/app";
  let name = "";
  let letters = /^[A-Za-z]+$/;

  function check() {
    // check the name to see if it's vaild
    if (name === "") {
      alert("please enter your name");
    } else if (name === " ") {
      alert("please enter your name");
    } else if (!name.match(letters)) {
      alert("please enter a name without numbers");
    } else if (name.length < 3) {
      alert("Please enter a name longer than 3 characters");
    } else if (name.length > 20) {
      alert("please enter a name less than 20 characters");
    } else {
      goto("./teams");
    }
  }
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
    margin-left: 80px;
    margin-top: 100px;
  }

  #dancer {
    margin-top: 100px;
    margin-left: 210px;
  }

  #relayrunner {
    margin-left: 150px;
    margin-top: 30px;
  }

  #basketballer {
    margin-left: 130px;
    margin-top: 30px;
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

  h1 {
    margin-top: 50px;
    font-size: 50px;
    color: #ffc600;
  }
</style>

<section>

  <header>
    <h1 class="title has-text-centered">Rangi Ruru Weekly Basketball Signup</h1>
  </header>

  <nav>
    <input bind:value={name} placeholder="Name" />

    {#if name}
      <p>Hello {name}</p>
    {:else}
      <p>Please enter your name.</p>
    {/if}

    <button on:click={check}>Next</button>

  </nav>

  <img id="dancer" src="/Dancer.png" alt="Dancer" />
  <img id="relayrunner" src="/Relay.png" alt="Relay runner" />
  <img id="basketballer" src="/Basketball.png" alt="Basketballer" />
  <img id="hockeyplayer" src="/Hockey.png" alt="Hockey player" />

</section>
