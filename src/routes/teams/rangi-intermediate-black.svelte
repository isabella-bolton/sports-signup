<script>
    let players = [
    {
   name: "Sophie Fulton",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Daisy Summerfield",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Lucinda Turnball",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Lucy Leech",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Maggie Craw",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Primrose Porter",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Gemma Beckett",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Holly Lill",
   playing: false,
   transportThere: false,
   transportBack: false,
  },

  {
   name: "Lily Parkinson",
   playing: false,
   transportThere: false,
   transportBack: false,
  },

  {
   name: "Millie Bushell",
   playing: false,
   transportThere: false,
   transportBack: false,
  },

  {
   name: "Emily Smith",
   playing: false,
   transportThere: false,
   transportBack: false,
  },

  {
      name: "Lucy Moffat",
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