<script>
  /* stores they players names and if they're playing and if they're getting transport there and back
   */
  let players = [
    {
      name: "Alice Wallis",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Phoebe Wallis",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Georgie Bethel",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Zara Frost",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Zara Stewart",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Nicole Vance",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Bex Skinner",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Florence Nelson",
      playing: false,
      transportThere: false,
      transportBack: false
    }
  ];
</script>

<!-- Each player gets a playing checkbox next to it-->
{#each players as player}
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
{/each}
<a class="button" href="teams">Back</a>

<img src="/logo.png" alt="RRGS logo" />
