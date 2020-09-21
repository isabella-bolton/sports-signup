<script>
  /* stores they players names and if they're playing and if they're getting transport there and back
   */
  let players = [
    {
      name: "Emma Ffowcs Williams",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Emma McCusker",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Lucy Vaughan",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Liv Armitage",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Chloe Hughes",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Camile Perelini",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Alice Edwards",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Harriet Fletcher",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Kate Harding",
      playing: false,
      transportThere: false,
      transportBack: false
    },

    {
      name: "Elsie Westphall",
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
