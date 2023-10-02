<script>
	import Repository from '../../components/organisms/Repository.svelte';
	const repos = [
		{
			name: 'Termux Theme Changer',
			description: 'A shell script to change the theme of termux app',
			src: 'https://github.com/youaremagic/termux-theme-changer'
		},
		{
			name: 'Repo Lang Stat',
			description:
				'Small cli line tool written in rust to get the statistics of programming languages used in a github repository',
			src: 'https://github.com/youaremagic/repo-lang-stat'
		}
	];
</script>

<div>
	{#each repos as repo}
		<Repository {...repo} />
	{/each}
</div>

<style scoped>
	div {
		display: flex;
		flex-direction: column;
		gap: 10px;
	}
</style>
