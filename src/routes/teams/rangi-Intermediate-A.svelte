<script>
/* stores they players names and if they're playing and if they're getting transport there and back
*/
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