<script>
	export let className = '';
</script>

<section class={className}><div class="mobileFirst"><slot /></div></section>

<style lang="scss">
	section {
		display: flex;
		justify-content: center;
		height: 600px;
		width: 100vw;
	}
</style>
