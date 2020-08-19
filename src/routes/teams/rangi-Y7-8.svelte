
<script>
    let players = [
    {
   name: "Annabel Strotton",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Tabitha Porter",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Ava-Bella Stowers",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Miriana Hansen",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Amelie Wilke",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Alania Perkins",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Evelyn Stewart",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Sophie Percy",
   playing: false,
   transportThere: false,
   transportBack: false,
  },

  {
   name: "Sophie Mounce",
   playing: false,
   transportThere: false,
   transportBack: false,
  },

  {
   name: "Joanna Yang",
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