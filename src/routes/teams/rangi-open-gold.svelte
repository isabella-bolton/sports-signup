<script>
    let players = [
    {
   name: "Leila Rhodes",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Harriet Fleury",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Emma Osteen",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Georgia Thompson",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Sammie Senior",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Kate Wield",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Rosa Blake",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Rosa Dalzell",
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
  