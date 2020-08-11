<script>
    let players = [
    {
   name: "Billie Edwards",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Alice Jones",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Lily Barrrowcliffe",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Rebecca Harvey",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Tessa Shield",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Madeline Haugh",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Lily Boock",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Mihiroa Pauling",
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
  