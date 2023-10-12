<script lang="ts">
	export let quote = '';
	export let remarks = '';
</script>

<div>
	<q>{quote}</q>
	<p>{remarks}</p>
</div>

<style lang="scss" scoped>
	@import '../../styles/variables.scss';
	$padding: 20px;
	div {
		width: calc(100% - 2 * $padding);
		padding: $padding;
		background-color: $box-color;
		border-radius: 5px;
	}
</style>
