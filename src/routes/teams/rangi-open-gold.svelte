<script>
/* stores they players names and if they're playing and if they're getting transport there and back
*/
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
  
  <!-- Each player gets a playing checkbox next to it-->  
  {#each players as player}
    <p>{player.name}</p>
  
    <label>
      <input type="checkbox" bind:checked={player.playing} />
      I am playing.
    </label>
  
    <!--  If the player ticks playing, then add transport there and back boxes -->
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