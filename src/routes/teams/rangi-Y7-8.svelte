<script>
/* stores they players names and if they're playing and if they're getting transport there and back
*/
  let players = [
    {
      name: "Annabel Strotton",
      playing: false,
      transportThere: false,
      transportBack: false
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
