<script>
	let name = '';
</script>

<style>
</style>

<h1 class="title is-1 title has-text-centered">Rangi Ruru Weekly Basketball Signup</h1>


<input bind:value={name} placeholder="Name">

{#if name}
	<p>Hello {name}</p>
{:else}
	<p>Please enter your name.</p>
{/if}

<a class="button" href="teams">
	Next
</a>