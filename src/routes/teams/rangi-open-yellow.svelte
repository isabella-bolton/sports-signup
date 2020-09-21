<script>
  /* stores they players names and if they're playing and if they're getting transport there and back
   */
  let players = [
    {
      name: "Holly O'Loughlin",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Brigit Moston",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Sophie Vryenhoek",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Franny Ullrich",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Sophie Pye",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Asta Kain",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Ella Newberry",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Elle Gurnsey",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Lauren Smith",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Katie Macleod",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Poppy Clark",
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
