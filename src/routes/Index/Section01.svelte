<script>
	import SectionDefault from '../../lib/Components/SectionDefault.svelte';

	function onClick() {
		alert('teste');
	}
</script>

<SectionDefault className="sec01">
	<div class="blurContent">
		<h1>Nós equipamos o seu negocio para o futuro</h1>
		<span>Com <strong>melhor</strong> que há a oferecer</span>
		<button on:click={onClick}>Quero saber mais!</button>
	</div>
</SectionDefault>

<style lang="scss">
	/* Especial */
	:global(.sec01) {
		background: url(../../lib/images/asset.png) center center no-repeat;
		background-size: cover;

		color: var(--color-main);
	}

	:global(.sec01 > .mobileFirst) {
		background-color: rgba(54, 54, 54, 0.6);
		backdrop-filter: blur(4.5px);
		display: flex;
		align-items: center;
		justify-content: center;
	}

	.blurContent {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;

		h1 {
			text-align: center;
			font-size: 60px;
			width: 510px;
			margin: 0;
			padding: 0;
		}

		span {
			font-size: 1.75rem;
			margin: 2rem;
			font-weight: 400;
		}

		button {
			font-family: var(--font-body);
			background-color: var(--color-main);
			color: var(--color-accent);
			border: none;
			font-size: 1.1rem;
			padding: 0.5rem 2rem;
			border-radius: 8px;
			font-weight: 600;
			cursor: pointer;
		}
	}
</style>
