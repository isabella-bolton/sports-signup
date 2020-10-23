<script>
  /* stores they players names and if they're playing and if they're getting transport there and back
   */
  let players = [];

  /*Saves data to local*/
  function savedata() {
    // let data = JSON.stringify(players);
    let data = {
      players: players
    };

    // save the person object to the database under their first name

    db.collection("players")
      .doc("openGreenplayers")
      .set(data);
  }

  /*Gets data from local*/
  async function getdata() {
    console.log("Getting the data");

    let data = await db
      .collection("players")
      .doc("openGreenplayers")
      .get();
    console.log("Got the data.");
    data = data.data();
    if (data == undefined) {
      console.log("Data is undefined");
      players = [
        {
          name: "Harriet Graham",
          playing: false,
          transportThere: false,
          transportBack: false
        },

        {
          name: "Jasmine Strawbridge",
          playing: false,
          transportThere: false,
          transportBack: false
        },

        {
          name: "Elizabeth Dooley",
          playing: false,
          transportThere: false,
          transportBack: false
        },

        {
          name: "Sophie Barnes",
          playing: false,
          transportThere: false,
          transportBack: false
        },

        {
          name: "Frankie Reid",
          playing: false,
          transportThere: false,
          transportBack: false
        },

        {
          name: "Mia Roadley",
          playing: false,
          transportThere: false,
          transportBack: false
        },

        {
          name: "Penny Proctor",
          playing: false,
          transportThere: false,
          transportBack: false
        },

        {
          name: "Penny Frost",
          playing: false,
          transportThere: false,
          transportBack: false
        },

        {
          name: "Jorja Tuanui",
          playing: false,
          transportThere: false,
          transportBack: false
        },

        {
          name: "Eva Matthews",
          playing: false,
          transportThere: false,
          transportBack: false
        },

        {
          name: "Simmone Cox",
          playing: false,
          transportThere: false,
          transportBack: false
        }
      ];
    } else {
      console.log("Data was found");
      //players = JSON.parse(data);
      players = data.players;
    }
  }

  getdata();
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

    button{
    margin-bottom: 30px;
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
    <button class="button" on:click={savedata}>Save</button>
    <a class="button" href="output">Players</a>

  </main>
</section>
