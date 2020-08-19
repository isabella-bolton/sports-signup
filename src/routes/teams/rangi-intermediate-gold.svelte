<script>
    let players = [
    {
   name: "Alice Wallis",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Phoebe Wallis",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Georgie Bethel",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Zara Frost",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Zara Stewart",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Nicole Vance",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Bex Skinner",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Florence Nelson",
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