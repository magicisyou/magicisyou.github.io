<script>
	export let name = 'Name';
	export let description = 'Description';
	export let src = '';
	export let image_url = '';
</script>

<div class="main_div">
	<div class="details_div">
		<h3>{name}</h3>
		<p>{description}</p>
		<a href={src} target="_blank">See github repository</a>
	</div>
	<div class="image_container">
		{#if image_url != ''}
			<img src={image_url} alt={name} />
		{/if}
	</div>
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
	.main_div {
		display: flex;
		flex-direction: row;
		align-items: flex-start;
		justify-content: space-between;
		background-color: $box-color;
		padding: 30px;
		border-radius: 5px;
		height: 200px;
	}
	.details_div {
		gap: 20px;
		display: flex;
		flex-direction: column;
		align-items: flex-start;
		width: 70%;
	}
	.image_container {
		width: 25%;
		height: 90%;
		display: flex;
		align-items: center;
		justify-content: center;
	}
	img {
		width: 100%;
		height: auto;
		max-height: 100%;
	}
	@media (max-width: 650px) {
		.main_div {
			flex-direction: column;
			height: auto;
			gap: 20px;
		}
		.image_container {
			width: 100%;
			height: auto;
		}
		.details_div {
			width: 100%;
		}
	}
</style>
