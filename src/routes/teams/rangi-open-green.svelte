<script>
    let players = [
    {
   name: "Harriet Graham",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Jasmine Strawbridge",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Elizabeth Dooley",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Sophie Barnes",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Frankie Reid",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Mia Roadley",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Penny Proctor",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Penny Frost",
   playing: false,
   transportThere: false,
   transportBack: false,
  },

  {
   name: "Jorja Tuanui",
   playing: false,
   transportThere: false,
   transportBack: false,
  },

  {
   name: "Eva Matthews",
   playing: false,
   transportThere: false,
   transportBack: false,
  },

  {
   name: "Simmone Cox",
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