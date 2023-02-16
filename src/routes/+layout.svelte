<script>
	import Footer from '../lib/Components/Footer.svelte';
	import Header from '../lib/Components/Header.svelte';
	import './styles.css';
</script>

<div class="app">
	<Header />

	<main>
		<slot />
	</main>

	<Footer />
</div>

<style>
	.app {
		display: flex;
		flex-direction: column;
		min-height: 100vh;
		background-color: var(--color-bg-0);
	}

	main {
		flex: 1;
		display: flex;
		flex-direction: column;
		align-items: center;
		width: 100%;
		overflow-x: hidden;
		margin: 0 0;
		padding: 0;
	}
</style>
