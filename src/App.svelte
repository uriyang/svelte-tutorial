<script>
	let count = 0;

	function handleClick() {
		count += 1;
	}
	$: {
		console.log(`ths count is ${count}`);
		alert(`I SAID THE COUNT IS ${count}`);
	}

	$: {
		if (count >= 10) {
			alert(`count is dangerously high!`);
			count = 9;
		}
	}
</script>

<main>
	<button on:click={handleClick}>
		Clicked {count} {count === 1 ? 'time' : 'times' }
	</button>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		margin: 0 auto;
	}
</style>