<script>
	export let name = 'Name';
	export let description = 'Description';
	export let src = '';
</script>

<div>
	<h3>{name}</h3>
	<p>{description}</p>
	<a href={src} target="_blank">See github repository</a>
</div>

<style lang="scss" scoped>
	@import '../../styles/variables.scss';
	a {
		color: #276b96;
		text-decoration: none;
		&:hover {
			color: #377ba6;
		}
	}
	div {
		display: flex;
		flex-direction: column;
		align-items: flex-start;
		gap: 20px;
		background-color: #102931;
		padding: 30px;
		border-radius: 5px;
	}
</style>
