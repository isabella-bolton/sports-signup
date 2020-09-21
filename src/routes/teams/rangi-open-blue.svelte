<script>
  /* stores they players names and if they're playing and if they're getting transport there and back
   */
  let players = [
    {
      name: "Annabelle Jones",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Maddy Sheat",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Lilly Ellis",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Anna Casey",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Claudia Brown",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Holly Allred",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Emma Schroder",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Georgia Sheat",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Brooke Raitt",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Chloe Berge",
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
