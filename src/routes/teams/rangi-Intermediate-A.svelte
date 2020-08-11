<script>
    let players = [
    {
   name: "Freya Herdman",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Georgia Dann",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Catelyn Henderson Geddes",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Nyah Reweti",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Milly Harrison",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Milly Gallagher",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Charlotte O'Reilly",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Milly Greenslade",
   playing: false,
   transportThere: false,
   transportBack: false,
  },

  {
   name: "Charlie Gaiger",
   playing: false,
   transportThere: false,
   transportBack: false,
  },

  {
   name: "Eliza Miller",
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
  