<script>
  let y78Players;
  let data = localStorage.getItem("y78Players");
  y78Players = JSON.parse(data);
</script>

<h1>Year 7/8 team</h1>

{#each y78Players as player}
  <p>{player.name}</p>

  {#if player.playing}
    <p>Playing</p>
  {:else}
    <p>Not playing</p>
  {/if}

  {#if player.transportThere}
    <p>Transport there</p>
  {:else}
    <p>No transport there</p>
  {/if}

  {#if player.transportBack}
    <p>Transport back</p>
  {:else}
    <p>No transport back</p>
  {/if}
{/each}

<!--
player
  - name
  - playing
  - transportThere
  - transportBack
-->
