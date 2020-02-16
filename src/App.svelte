<script>
	let count = 0;

	function handleClick() {
		count += 1;
	}
</script>

<main>
	<button on:click={handleClick}>
	Clicked {count} {count === 1 ? 'time' : 'times' }</button>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		margin: 0 auto;
	}
</style>