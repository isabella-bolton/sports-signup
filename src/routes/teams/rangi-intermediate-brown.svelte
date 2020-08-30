<script>
/* stores they players names and if they're playing and if they're getting transport there and back
*/
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