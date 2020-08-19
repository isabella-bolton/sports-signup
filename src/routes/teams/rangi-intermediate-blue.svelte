<script>
  let players = [
  {
 name: "Kate Gourley",
 playing: false,
 transportThere: false,
 transportBack: false,
},

{
 name: "Livi Godfrey",
 playing: false,
 transportThere: false,
 transportBack: false,
},

{
 name: "Libby Ward",
 playing: false,
 transportThere: false,
 transportBack: false,
},

{
 name: "Sadie Lee",
 playing: false,
 transportThere: false,
 transportBack: false,
},

{
 name: "Ella Hartel",
 playing: false,
 transportThere: false,
 transportBack: false,
},

{
 name: "Siara Harmon",
 playing: false,
 transportThere: false,
 transportBack: false,
},

{
 name: "Issy Stiles",
 playing: false,
 transportThere: false,
 transportBack: false,
},

{
 name: "Georgia Gaiger",
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
    I am playing.
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
  <a class="button" href="teams">
	Back
</a>