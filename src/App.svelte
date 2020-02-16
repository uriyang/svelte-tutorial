<script>
	let string = `this string contains some <strong>HTML!!!</strong>`;
</script>

<main>
	<h1>{@html string}</h1>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		font-weight: normal;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>