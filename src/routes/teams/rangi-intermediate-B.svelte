<script>
    let players = [
    {
   name: "Briana Hodgen",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Nina Cantos",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Henrietta Evatt",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Lily Nimmo",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Sophie Payne",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Sophie Cusiel",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Imogen Savage",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Anna Wyn-Harris",
   playing: false,
   transportThere: false,
   transportBack: false,
  },

  {
   name: "Stuti Hari",
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
