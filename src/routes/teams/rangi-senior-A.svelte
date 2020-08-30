<script>
/* stores they players names and if they're playing and if they're getting transport there and back
*/
    let players = [
    {
   name: "Charlotte Gray",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Rosie Gray",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Abby Kneebone",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Elisha Vili Umaga",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Serena Tarawa",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Harriet Rance",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Claudia O'Shannessey",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Dayna Simpson",
   playing: false,
   transportThere: false,
   transportBack: false,
  },

  {
   name: "Molly Kneebone",
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