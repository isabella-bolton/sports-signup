<script>
  /* stores they players names and if they're playing and if they're getting transport there and back
   */
  let players = [
    {
      name: "Rebecca Harvey",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Gabby Cusiel",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Holly White",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Meg Crump",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Evie Laidlaw",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Sophia Watts",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Claudie Moore",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Jasmin Goodwillie",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Sienna O'Shannessey",
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
