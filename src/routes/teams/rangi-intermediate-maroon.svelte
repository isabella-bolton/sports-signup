<script>
    let players = [
    {
   name: "Molly Penberthy",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Riley Pirie",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Mya Wolfenden",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Aggie Weston",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Hayley Bond",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Polly Cross",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Tilly Hlavac",
   playing: false,
   transportThere: false,
   transportBack: false,
  },
  
  {
   name: "Brooke Summerfield",
   playing: false,
   transportThere: false,
   transportBack: false,
  },

  {
   name: "Alyssa Astle",
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
      playing, I am playing.
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
  