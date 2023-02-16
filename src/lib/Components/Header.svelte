<script>
	import { page } from '$app/stores';

	import logoImg from '$lib/images/Logo.svg';
	import telImg from '$lib/images/tel.svg';
	import wppImg from '$lib/images/wpp.svg';
	import emailImg from '$lib/images/email.svg';
	import PhoneDiv from './PhoneDiv.svelte';
</script>

<header>
	<div class="mobileFirst space-between">
		<div class="corner">
			<img src={logoImg} alt="logo" />
			<div class="center column">
				<h1 id="header_title">Regi</h1>
				<span id="header_subtitle">Maquinas e Equipamentos</span>
			</div>
		</div>
		<div class="corner column space-between">
			<nav>
				<PhoneDiv />
				<a href="#Parceiros"><img src={wppImg} alt="WhatsApp" /> </a>
				<a href="#Parceiros"><img src={emailImg} alt="Email" /></a>
			</nav>
			<nav class="internlinks">
				<a href="#Inicio">Inicio</a>
				<a href="#Parceiros">Parceiros</a>
				<a href="#SobreNos">Sobre nós</a>
			</nav>
		</div>
	</div>
</header>

<style lang="scss">
	header {
		display: flex;
		justify-content: center;
		padding: 8px;

		.corner {
			display: flex;
		}

		img {
			width: 5rem;
			aspect-ratio: 1/1;
		}

		nav {
			display: flex;
			align-items: flex-end;
			justify-content: flex-end;

			& > * {
				display: flex;
				justify-content: center;
				align-items: center;
				padding-right: 1rem;

				span {
					padding: 0 8px;
				}

				img {
					aspect-ratio: 1/1;
					width: 2rem;
				}
			}
		}

		nav.internlinks {
			justify-content: space-between;

			a {
				font-size: 1.15rem;
				color: var(--color-accent);
				text-decoration: none;
				font-weight: 500;
				padding: 0 1rem;
				text-transform: uppercase;
				border-bottom: solid 4px transparent;
				transition: 0.2s all;

				&:hover {
					border-bottom: solid 4px var(--color-title-0);
					background-color: var(--color-bg-0);
				}
			}
		}
	}

	#header_title {
		display: flex;
		font-size: 3rem;
		margin: 0px;
		margin-block: 0px;
		margin-inline: 0px;
		text-transform: uppercase;
		color: var(--color-title-0);
		font-family: var(--font-title);
		line-height: 3rem;
	}

	#header_subtitle {
		font-size: 1.25rem;
		font-weight: 300;
		margin: none;
		padding: 0;
		text-transform: uppercase;
		color: var(--color-subtitle-0);
		font-family: var(--font-subtitle);
	}
</style>
