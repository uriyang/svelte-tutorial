<script>
	import Nested from './Nested.svelte';
</script>

<main>
	<Nested answer={42} />
	<Nested />
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		margin: 0 auto;
	}
</style>