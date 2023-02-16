<script>
	import beckerImg from '../../lib/images/Providers_Image/png/becker.png';
	import geloparImg from '../../lib/images/Providers_Image/png/gelopar.png';
	import guralImg from '../../lib/images/Providers_Image/png/gural.png';
	import innalImg from '../../lib/images/Providers_Image/png/innal.png';
	import metvisaImg from '../../lib/images/Providers_Image/png/metvisa.png';
	import polarImg from '../../lib/images/Providers_Image/png/polar.png';
	import polofrioImg from '../../lib/images/Providers_Image/png/polofrio.png';
	import progasImg from '../../lib/images/Providers_Image/png/progas.png';
	import uranoImg from '../../lib/images/Providers_Image/png/urano.png';
	import venancioImg from '../../lib/images/Providers_Image/png/venancio-metal.png';
	import venaxImg from '../../lib/images/Providers_Image/png/venax.png';

	var imgArr = [
		beckerImg,
		geloparImg,
		guralImg,
		innalImg,
		metvisaImg,
		polarImg,
		polofrioImg,
		progasImg,
		uranoImg,
		venancioImg,
		venaxImg
	];
	// import progasImg from '../../lib/images/Providers_Image/png/progas.png';
</script>

<section id="ourPartners">
	<div class="mobileFirst">
		<h1>Nossos Parceiros</h1>
		<div class="imgGrid">
			{#each imgArr as srcArr, i}
				<img src={srcArr} />
			{/each}
		</div>
	</div>
</section>

<style lang="scss">
	#ourPartners {
		padding: 3rem;

		div {
			display: flex;
			flex-direction: column;
			justify-content: center;
			align-items: center;

			h1 {
				font-weight: 600;
				font-size: 2.5rem;
				color: var(--color-accent);
				margin: 2rem;
				border-bottom: 2px solid var(--color-accent);
			}
		}

		.imgGrid {
			columns: 2;
			display: grid;
			justify-items: center;
			align-items: center;
			grid-template-columns: repeat(3, 1fr);
			gap: 1rem 3rem;
			grid-auto-rows: auto;

			img {
				break-inside: avoid;
				height: 4rem;
			}
		}
	}
</style>
