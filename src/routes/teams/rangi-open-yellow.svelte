<script>
    let players = [
    {
   name: "Holly O'Loughlin",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Brigit Moston",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Sophie Vryenhoek",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Franny Ullrich",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Sophie Pye",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Asta Kain",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Ella Newberry",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Elle Gurnsey",
   playing: false,
   transportThere: false,
   transportBack: false,
  },

  {
   name: "Lauren Smith",
   playing: false,
   transportThere: false,
   transportBack: false,
  },

  {
   name: "Katie Macleod",
   playing: false,
   transportThere: false,
   transportBack: false,
  },

  {
   name: "Poppy Clark",
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