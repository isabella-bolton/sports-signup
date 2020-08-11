<script>
    let players = [
    {
   name: "Rebecca Harvey",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Gabby Cusiel",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Holly White",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Meg Crump",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Evie Laidlaw",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Sophia Watts",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Claudia Moore",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Jasmin Goodwille",
   playing: false,
   transportThere: false,
   transportBack: false,
  },

  {
   name: "Sienna O'Shannessey",
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
  