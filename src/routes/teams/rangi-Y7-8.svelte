<script>
  /* stores they players names and if they're playing and if they're getting transport there and back
   */

  let players = [];

  /*Saves data to local*/
  function saveDataToLocal() {
    let data = JSON.stringify(players);
    localStorage.setItem("y78Players", data);
  }

  /*Gets data from local*/
  function getDataFromLocal() {
    console.log("Getting the data");
    let data = localStorage.getItem("y78Players");
    console.log("Got the data.");
    if (data == undefined) {
      console.log("Data is undefined");
      players = [
        {
          name: "Annabel Strotton",
          playing: false,
          transportThere: false,
          transportBack: false,
          notPlaying: ""
        },

        {
          name: "Tabitha Porter",
          playing: false,
          transportThere: false,
          transportBack: false
        },

        {
          name: "Ava-Bella Stowers",
          playing: false,
          transportThere: false,
          transportBack: false
        },

        {
          name: "Miriana Hansen",
          playing: false,
          transportThere: false,
          transportBack: false
        },

        {
          name: "Amelie Wilke",
          playing: false,
          transportThere: false,
          transportBack: false
        },

        {
          name: "Alania Perkins",
          playing: false,
          transportThere: false,
          transportBack: false
        },

        {
          name: "Evelyn Stewart",
          playing: false,
          transportThere: false,
          transportBack: false
        },

        {
          name: "Sophie Percy",
          playing: false,
          transportThere: false,
          transportBack: false
        },

        {
          name: "Sophie Mounce",
          playing: false,
          transportThere: false,
          transportBack: false
        },

        {
          name: "Joanna Yang",
          playing: false,
          transportThere: false,
          transportBack: false
        }
      ];
    } else {
      console.log("Data was found");
      players = JSON.parse(data);
    }
  }

  getDataFromLocal();
</script>

<style>
  /* ####### LAYOUT ####### */
  section {
    display: grid;
    grid-gap: 50px;
    grid:
      " header " auto
      " main   " auto
      / 1fr;
  }

  header {
    grid-area: header;
  }
  nav {
    grid-area: nav;
  }
  main {
    grid-area: main;
  }
  footer {
    grid-area: footer;
  }

  /* ####### STYLE ####### */
  nav {
    padding-top: 30px;
  }

  img {
    width: 200px;
  }
  header {
    background-color: #1e387c;
  }

  .player {
    margin-top: 30px;
    margin-left: 30px;
  }
</style>

<section>

  <header>
    <img src="/logo.png" alt="RRGS logo" />
  </header>

  <main>
    <!-- Each player gets a playing checkbox next to it-->
    {#each players as player}
      <div class="player">
        <p>{player.name}</p>

        <label>
          <input type="checkbox" bind:checked={player.playing} />
          I am playing.
        </label>

        <!--  If the player ticks playing, then add transport there and back boxes -->
        {#if player.playing}
          <label>
            <input type="checkbox" bind:checked={player.transportThere} />
            Transport there?
          </label>

          <label>
            <input type="checkbox" bind:checked={player.transportBack} />
            Transport back?
          </label>
        {/if}

        <!--  If the player doesn't tick anything, then ask why they're not playing -->
        {#if !player.playing}
          <p>Why are you unable to play?</p>
          <input bind:value={player.notPlaying} />
        {/if}
        <br />
      </div>
    {/each}

    <footer />
    <nav />

    <a class="button" href="teams">Back</a>
    <button class="button" on:click={saveDataToLocal}>Save</button>
    <a class="button" href="output">Players</a>

  </main>
</section>
