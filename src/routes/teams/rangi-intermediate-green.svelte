<script>
    let players = [
    {
   name: "Bridget Pye",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Arabella Acland",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Maddie Trolove",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Annabel Wynn-Williams",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Mary Flatman",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Alice Hunter",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Frankie Richards",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Eliza Frew",
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