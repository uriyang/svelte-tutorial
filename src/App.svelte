<script>
	let name = 'world'
	let src = 'https://svelte.dev/tutorial/image.gif'
</script>

<main>
	<h1>Hello {name}</h1>
	<img src={src} alt="dance" />
	<p>This is a paragraph.<p>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}

	p {
		color: purple;
		font-family: 'Comic Sans Ms', cursive;
		font-size: 2em;
	}
</style>