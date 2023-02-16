<script>
	import telImg from '$lib/images/tel.svg';
	export let inverted = false;
</script>

<div class={inverted ? 'invertImg PhoneDiv' : 'PhoneDiv'}>
	<img src={telImg} alt="WhatsApp" /><span>(91) 9 9999-9999</span>
</div>

<style lang="scss">
	.PhoneDiv {
		display: flex;
		justify-content: center;
		align-items: center;
		margin: 0 1rem;

		gap: 0.5rem;
	}

	.invertImg {
		img {
			filter: invert(100%);
		}
	}
</style>
