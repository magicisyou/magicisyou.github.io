<script>
	import Navigation from '../molecules/navigation.svelte';
</script>

<header>
	<Navigation />
</header>

<style lang="scss" scoped>
	@import '../../styles/variables.scss';

	header {
		position: sticky;
		top: 0;
		background-color: $background-color;
		margin-bottom: $header-and-footer-margin;
		padding: $header-and-footer-padding;
		height: $header-and-footer-height;
		width: calc(100% - 2 * #{$header-and-footer-padding});
	}
</style>
