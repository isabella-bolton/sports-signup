<script>
  let players = [
  {
 name: "Tayla Ferguson",
 playing: false,
 transportThere: false,
 transportBack: false,
},

{
 name: "Izzy Bolton",
 playing: false,
 transportThere: false,
 transportBack: false,
},

{
 name: "Lucy Howden",
 playing: false,
 transportThere: false,
 transportBack: false,
},

{
 name: "Brie Yates",
 playing: false,
 transportThere: false,
 transportBack: false,
},

{
 name: "Liv Jerard",
 playing: false,
 transportThere: false,
 transportBack: false,
},

{
 name: "Ruby Lee",
 playing: false,
 transportThere: false,
 transportBack: false,
},

{
 name: "Olivia Yankov-Reid",
 playing: false,
 transportThere: false,
 transportBack: false,
},

{
 name: "Cindy Luan",
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
