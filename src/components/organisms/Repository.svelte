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
		color: #6089ff;
		text-decoration: none;
		&:hover {
			color: #4069df;
		}
	}
	div {
		display: flex;
		flex-direction: column;
		align-items: flex-start;
		gap: 20px;
		background-color: $box-color;
		padding: 30px;
		border-radius: 5px;
	}
</style>
