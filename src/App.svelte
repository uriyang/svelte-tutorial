<script>
	let count = 0;

	$: doubled = count * 2;

	function handleClick() {
		count += 1;
	}
</script>

<main>
	<button on:click={handleClick}>
		Clicked {count} {count === 1 ? 'time' : 'times' }
	</button>
	<p>{count} doubled is {doubled}</p>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		margin: 0 auto;
	}
</style>