<script>
/* stores they players names and if they're playing and if they're getting transport there and back
*/
    let players = [
    {
   name: "Imogen Foote",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Emma Comerford",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Gracie Liu",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Danielle Milliken",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Riannon Holmnowsky",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Lotte Giesen",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Jess Glass",
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
