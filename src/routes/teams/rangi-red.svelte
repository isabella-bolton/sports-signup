<script>
  let players = [
    {
      name: "Lilly",
      playing: false,
      transportThere: false,
      transportBack: false,
    },
    {
      name: "Tayla",
      playing: false,
      transportThere: false,
      transportBack: false,
    },
  ]
</script>

{#each players as player}
  <p>{player.name}</p>

  <label>
    <input type="checkbox" bind:checked={player.playing} />
    playing, I am playing.
  </label>

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
