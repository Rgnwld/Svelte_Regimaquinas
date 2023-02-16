<script>
	import PhoneDiv from '$lib/Components/PhoneDiv.svelte';
	import SectionDefault from '../../lib/Components/SectionDefault.svelte';
	import MapImg from '$lib/images/map.png';
	import wppImg from '$lib/images/wpp.svg';
	import emailImg from '$lib/images/email.svg';
</script>

<SectionDefault className="sec02">
	<div class="sec02_container">
		<h1>Venha nos conhecer</h1>
		<div class="doubleColumn">
			<div class="side">
				<p>
					Se você estiver procurando uma <strong>empresa de equipamentos comerciais</strong>,
					gostaria de convidá-lo a visitar nossa loja verificar se há algo que possa atender às suas
					necessidades.
				</p>
				<p>
					Nós oferecemos <strong>preços competitivos, serviço ao cliente e entrega rápida</strong>.
					Esperamos ter a oportunidade de trabalhar com você!
				</p>
				<div class="buttonContainer">
					<PhoneDiv inverted />
					<div>
						<button>Entre em contato</button>
						<a href="#Parceiros"><img src={wppImg} alt="WhatsApp" /> </a>
						<a href="#Parceiros"><img src={emailImg} alt="Email" /></a>
					</div>
				</div>
				<div />
			</div>
			<div class="side mapContainer" />
		</div>
	</div>
</SectionDefault>

<style lang="scss">
	:global(.sec02) {
		color: var(--color-main);
		background-color: var(--color-accent);
	}

	.sec02_container {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		height: 100%;

		h1 {
			font-size: 60px;
		}

		.doubleColumn {
			display: flex;
			width: 100%;

			gap: 3rem;

			& > .side {
				display: flex;
				flex-direction: column;
				width: 100%;

				& > .buttonContainer {
					display: flex;
				}

				p {
					text-align: justify;
					text-indent: 50px;
					font-size: 1.3rem;
				}

				img {
					/* height: 10rem;
					 */
				}
			}
		}
	}
</style>
