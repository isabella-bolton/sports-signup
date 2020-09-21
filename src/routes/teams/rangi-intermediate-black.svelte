<script>
  /* stores they players names and if they're playing and if they're getting transport there and back
   */
  let players = [
    {
      name: "Sophie Fulton",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Daisy Summerfield",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Lucinda Turnball",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Lucy Leech",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Maggie Craw",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Primrose Porter",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Gemma Beckett",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Holly Lill",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Lily Parkinson",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Millie Bushell",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Emily Smith",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Lucy Moffat",
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
