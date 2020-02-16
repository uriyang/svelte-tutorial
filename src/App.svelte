<script>
	let numbers = [1, 2, 3, 4];

	function addNumber() {
		// # type 1
		// numbers.push(numbers.length + 1);
		// numbers = numbers;

		// # type 2
		// numbers = [...numbers, numbers.length + 1]

		// # type 3
		numbers[numbers.length] = numbers.length + 1

	}

	$: sum = numbers.reduce((t, n) => t + n, 0)
</script>

<main>
	<p>{numbers.join(' + ')} = {sum}</p>
	<button on:click={addNumber}>
		Add a number
	</button>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		margin: 0 auto;
	}
</style>